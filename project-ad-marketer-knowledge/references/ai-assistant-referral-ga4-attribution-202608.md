# LLM·AI 추천 유입의 GA4 측정 원칙

확인일: 2026-08-18

## 1) 새로 학습한 사실

- Google Analytics는 2026-05-13부터 인식 가능한 AI 도우미 리퍼러에 매체 `ai-assistant`, 기본 채널 `AI Assistant`, 캠페인 `(ai-assistant)`를 자동 부여한다. Google이 예시로 밝힌 서비스는 ChatGPT, Gemini, Claude이며 전체 인식 목록은 공개하지 않았다.
- GA4 커스텀 채널 그룹은 보고서와 탐색 분석에서 과거 데이터에도 적용할 수 있다. 다만 이를 속성의 기본 `Primary channel group`으로 지정한 이후의 기본 채널 기록은 향후 데이터부터 채워진다.
- Google은 커스텀 채널 그룹의 AI 도우미 예시를 공식 도움말에 제공한다. AI 채널을 Referral보다 위에 배치해야 먼저 분류된다.
- Google Search의 AI Overview·AI Mode에서 발생한 노출과 클릭은 Google Search 트래픽에 포함된다. 따라서 Gemini 웹·앱의 직접 추천 유입과 Google 검색결과의 AI 기능 유입은 측정 범위가 다르다.
- Search Console에는 Google Search의 AI Overview·AI Mode 노출을 확인하는 생성형 AI 성과 보고서가 순차 제공되고 있다. GA4의 `AI Assistant` 채널만으로는 Google 검색 내 AI 기능의 가시성을 분리할 수 없다.
- 2026-08-18 현재 Search Console 생성형 AI 성과 보고서는 AI Overview·AI Mode의 `노출`을 페이지·국가·날짜·기기 기준으로 보여준다. AI 기능 클릭을 GA4 세션과 일대일 연결하는 식별자는 제공하지 않는다.

공식 근거:

- Google Analytics 새로운 AI 도우미 트래픽 측정: https://support.google.com/analytics/answer/9164320#05132026
- GA4 커스텀 채널 그룹 및 AI 도우미 예시: https://support.google.com/analytics/answer/13051316
- GA4 기본 채널 그룹 정의: https://support.google.com/analytics/answer/9756891
- Google Search AI 기능 측정: https://developers.google.com/search/docs/appearance/ai-features
- Search Console 생성형 AI 성과 보고서: https://support.google.com/webmasters/answer/16984139

## 2) 기존 지식에서 수정할 점

- `LLM이 만든 외부 링크에는 광고주가 UTM을 임의로 붙일 수 없다`는 설명은 일반적으로 맞다. 다만 모든 AI 서비스가 항상 UTM을 붙이지 않는다고 영구적으로 단정하지 않는다. 서비스별 링크 정책과 실제 클릭 URL은 변경될 수 있다.
- Claude 유입이 항상 `claude.ai/referral` 또는 날짜가 포함된 경로로 전달된다는 주장은 공식 확인이 되지 않았다. GA4의 `세션 소스`에는 일반적으로 `claude.ai`처럼 호스트명이 표시될 수 있으므로 전체 리퍼러 경로는 브라우저 실측이나 서버 로그로 확인한다.
- 리퍼러가 사라진 AI 유입의 비율을 `35~70%`처럼 공통 수치로 제시하지 않는다. 앱, 브라우저, 이동 방식, 개인정보 설정에 따라 달라지며 신뢰할 수 있는 공통 공식값이 없다.
- `AI Assistant` 기본 채널이 과거 데이터를 재분류하지 않는다는 설명과 커스텀 채널 그룹의 소급 적용을 혼동하지 않는다. 기본 채널의 자동 분류는 도입 이후 수집값을 중심으로 보고, 커스텀 채널 그룹은 이미 저장된 Source·Medium 값에 규칙을 과거 범위로 적용할 수 있다.
- Google AI Overview·AI Mode 유입을 `AI Assistant`로 집계한다고 설명하지 않는다. 이 트래픽은 Google Search 측정 범위이며 Search Console과 GA4 Organic Search를 함께 본다.
- Search Console을 GA4에 연결해도 개별 GA4 세션에 `AI Overview 클릭` 표시가 붙는다고 설명하지 않는다. 연결 보고서는 Search Console의 검색 전 단계 집계와 GA4의 방문 후 행동을 방문 페이지·기기·국가 수준에서 함께 보는 구조다.
- 네이버 AI 브리핑·AI탭에서 외부 사이트를 클릭한 방문을 GA4나 네이버 서치어드바이저에서 별도 AI 채널로 자동 분류할 수 있다고 주장하지 않는다. 현재 공식 서치어드바이저 문서는 웹 검색 관련 영역의 노출·클릭 합계만 안내한다.

## 3) 실무 적용 원칙

### 3.1 기본 측정 구조

1. GA4 `보고서 → 획득 → 트래픽 획득`에서 `세션 기본 채널 그룹`의 `AI Assistant`를 확인한다.
2. 보조 측정기준으로 `세션 소스/매체`, `세션 캠페인`, `방문 페이지 + 쿼리 문자열`을 추가해 AI 서비스별 유입과 전환을 확인한다.
3. 커스텀 채널 그룹에 AI 유입 채널을 만들고 Referral보다 위에 둔다.
4. 커스텀 채널은 과거 Source·Medium 값의 재분류와 기본 채널에서 빠진 알려진 AI 도메인의 보완용으로 사용한다.
5. `AI Assistant` 기본 채널과 커스텀 AI 채널을 나란히 비교하되 합산 시 중복되지 않도록 같은 채널 그룹 안에서 우선순위를 관리한다.

### 3.2 권장 정규식

GA4 `Source`가 호스트명 형태로 저장된 경우 다음처럼 정확한 도메인과 정상 서브도메인을 묶을 수 있다.

```regex
(^|\.)(chatgpt\.com|chat\.openai\.com|claude\.ai|perplexity\.ai|gemini\.google\.com|copilot\.microsoft\.com)$
```

- `(^|\.)`는 문자열 시작 또는 정상 서브도메인 경계를 뜻한다.
- `$`는 도메인 뒤에 다른 문자열이 붙는 오탐을 줄인다.
- 실제 GA4에 저장된 Source 값과 Google의 인식 목록은 바뀔 수 있으므로 월 1회 `세션 소스/매체`의 신규 리퍼러를 확인해 규칙을 갱신한다.
- Google 공식 도움말의 예시 정규식은 포괄적이어서 `ai`, `gpt` 같은 문자열이 포함된 일반 도메인까지 오탐할 수 있다. 광고주 보고용 규칙은 실제 유입 Source 목록을 바탕으로 더 보수적으로 만든다.

### 3.3 추가 측정 방법

- 서버·CDN 로그: 요청 헤더의 `Referer`, 방문 URL, 시간, 사용자 에이전트를 확인한다. GA4 태그 차단·동의 거부 시의 방문을 일부 보완하지만 리퍼러가 처음부터 없으면 AI 출처를 복원할 수 없다.
- 브라우저 실측: 각 AI 서비스의 웹·앱에서 링크를 직접 클릭하고 GA4 실시간·DebugView, 브라우저 개발자도구, 서버 로그를 동시에 확인한다. 서비스와 기기별로 최소 1회 검증한다.
- 원본 리퍼러 저장: 사이트에서 브라우저가 제공한 `document.referrer`를 GTM으로 읽어 이벤트 매개변수나 사용자 정의 측정기준에 저장할 수 있다. 전체 경로가 제공될 때만 세부 경로를 분석할 수 있으며, 비어 있는 리퍼러를 복구하지는 못한다. 개인정보 처리방침과 수집 범위를 함께 검토한다.
- BigQuery: GA4 원시 내보내기에서 세션 소스·매체와 랜딩·전환 이벤트를 결합해 장기 추세를 분석한다. GA4 커스텀 채널 그룹 자체는 BigQuery 내보내기에 포함되지 않으므로 SQL에서 동일 규칙을 재현한다.
- Google Search Console: AI Overview·AI Mode는 생성형 AI 성과 보고서가 제공되는 속성에서 노출을 확인하고, GA4 Organic Search의 방문·전환과 함께 본다.
- Google Search Console와 GA4 연결: `Google Organic Search Traffic` 보고서에서 방문 페이지별 Search Console 지표와 GA4 참여·전환 지표를 나란히 볼 수 있다. 이는 집계 수준의 비교이며 AI 기능에서 발생한 개별 세션을 판별하거나 전환에 확정 귀속하는 기능은 아니다.
- Google AI 기능의 근사 분석: 동일 날짜·방문 페이지·기기·국가 단위로 Search Console 생성형 AI 노출 변화와 GA4 `google / organic` 세션·전환 변화를 비교한다. 상관관계 분석일 뿐 AI Overview 유입 건수나 전환을 확정하지 않는다.
- 네이버 AI 브리핑·AI탭: GA4에서는 일반적으로 `naver / organic` 범위에 포함될 가능성이 높다. 서치어드바이저의 웹 콘텐츠 노출·클릭과 GA4 방문 페이지·전환을 날짜·페이지 기준으로 비교하되, AI 브리핑 전용 구분값이 공식 제공되기 전에는 AI 유입으로 확정하지 않는다.
- 전환 폼 보조 질문: 중요한 상담·견적 서비스는 `처음 알게 된 경로`에 ChatGPT·Claude·Gemini·Perplexity·기타 AI를 선택지로 추가한다. 자기기입 자료이므로 GA4와 합산하지 않고 교차검증한다.
- 전용 랜딩 또는 고유 경로: 광고주가 직접 배포하는 AI용 안내 페이지나 제휴 링크에는 UTM 또는 고유 경로를 사용할 수 있다. 다만 LLM이 원문 URL을 그대로 인용한다는 보장이 없으므로 자연 추천 유입 전체의 측정 수단으로 보지 않는다.

### 3.4 한계와 보고 기준

- 리퍼러가 없는 방문은 대체로 Direct로 남아 AI 서비스별 출처를 확정할 수 없다.
- GA4 기본 AI 채널의 전체 인식 도메인은 공개되지 않아 커스텀 채널과 수치 차이가 생길 수 있다.
- 동일 사용자가 AI 추천을 본 뒤 검색하거나 URL을 직접 입력하면 마지막 세션의 획득 경로만으로 최초 AI 접점을 확인하기 어렵다.
- GA4·서버 로그·폼 응답은 측정 범위가 다르므로 하나의 숫자로 강제 합산하지 않는다. `GA4에서 확인된 AI 추천 유입의 최소 관측치`와 `보조 설문 응답`을 분리해 보고한다.

### 3.5 AI 인용·노출 통합 대시보드

하나의 대시보드로 통합하는 것은 가능하지만 지표의 증거 수준을 구분한다.

| 단계 | 지표 | 의미 | 자동 수집 가능성 |
|---|---|---|---|
| A. 공식 노출 | Search Console 생성형 AI 노출 | Google AI Overview·AI Mode에 URL이 실제 표시됨 | UI 내보내기는 가능. 전용 API 제공은 공식 문서에서 확인되지 않아 계정별 API 응답 검증 필요 |
| B. 직접 관측 인용 | 정해진 질문에서 브랜드·URL 인용 확인 | 해당 시점·질문·환경에서 실제 인용됨 | 공식 소비자 서비스 API가 없으면 정기 수동 표본조사 또는 허용된 API 필요 |
| C. 크롤링 | AI 봇·검색봇의 URL 요청 수 | 콘텐츠 발견·갱신 가능성 | 서버·CDN 로그에서 자동 집계 가능 |
| D. 추천 방문 | GA4 AI Assistant·리퍼러 | 인용 링크를 통해 실제 방문한 최소 관측치 | GA4 Data API·BigQuery로 자동화 가능 |

운영 원칙:

1. 봇 크롤링 수를 `인용 횟수`, `인용률`, `AI 점유율`로 이름 붙이지 않는다.
2. Googlebot 크롤링은 Google Search 수집 신호이며 AI Overview 인용을 증명하지 않는다.
3. 네이버 Yeti 크롤링도 네이버 검색 수집 신호이며 AI 브리핑·AI탭 인용을 증명하지 않는다.
4. Google 생성형 AI 보고서는 공식 노출 지표로 별도 저장한다. 현재 공식 안내는 UI 내보내기를 명시하지만 전용 API·Bulk Export 지원을 명시하지 않으므로 Search Analytics API의 `searchAppearance` 값을 실제 속성에서 조회해 자동화 가능 여부를 검증한다.
5. Search Analytics API에서 생성형 AI 전용 값이 반환되지 않으면 CSV 정기 업로드를 사용하고 로그인 화면 자동화는 UI 변경·약관·인증 위험 때문에 최후 수단으로 둔다.
6. 네이버 서치어드바이저에는 공개된 AI 브리핑 전용 API·측정기준이 확인되지 않았다. 웹 검색 노출·클릭은 전체 검색 지표로 보관하고 AI 브리핑 관측치는 별도 수동 표본조사로 관리한다.
7. 대시보드의 종합점수는 서로 다른 지표를 단순 합산하지 않는다. `공식 노출`, `관측 인용`, `크롤링`, `추천 방문`을 별도 카드와 추세선으로 표시한다.

권장 데이터 구조:

- `crawler_log_daily`: 날짜, 봇명, URL, 요청 수, 상태코드, 마지막 크롤링 시각
- `google_ai_impression_daily`: 날짜, URL, 국가, 기기, AI 노출 수, 수집 방식
- `observed_citation_check`: 확인일, 서비스, 질문, 브랜드 언급, URL 인용, 순서, 증빙 화면
- `ai_referral_session_daily`: 날짜, AI 소스, 방문 페이지, 세션, 주요 이벤트, 전환
- `naver_search_visibility_daily`: 날짜, URL, 전체 웹 검색 노출·클릭, AI 브리핑 관측 여부, 수집 방식

권장 구현:

`서버·CDN 로그 + GA4 Data API 또는 BigQuery + Search Console 수집 + 수동 관측 업로드 → BigQuery/PostgreSQL → Looker Studio·Power BI·Metabase`

대시보드 명칭도 `AI 인용 지수`보다 `AI 검색·추천 가시성 대시보드`가 안전하다. 종합지수가 필요하면 각 하위지표와 가중치, 데이터 누락 여부를 공개하고 공식 인용 점유율처럼 표현하지 않는다.

## 4) 제안서/리포트 문장 예시

> ChatGPT·Claude·Gemini 등 인식 가능한 AI 도우미에서 발생한 방문은 GA4의 `AI Assistant` 채널과 세션 소스 기준으로 확인하겠습니다. 다만 앱·브라우저 환경에서 리퍼러가 전달되지 않은 방문은 Direct로 분류될 수 있어, 수치는 전체 AI 추천 유입이 아닌 확인 가능한 최소 범위로 해석합니다.

> Google AI Overview·AI Mode의 노출은 일반 AI 도우미 추천 유입과 분리해 Search Console 생성형 AI 성과 보고서에서 확인하고, 실제 방문과 전환은 GA4의 Google Organic Search 데이터와 교차 분석하겠습니다.

> 상담·견적 전환이 중요한 경우 GA4 유입 정보와 상담 폼의 `최초 인지 경로` 응답을 함께 확인해, AI 추천이 직접 방문·브랜드 검색으로 이어진 간접 효과까지 보완적으로 판단하겠습니다.

## 5) 다음 확인 필요사항

- 해당 GA4 속성에 `AI Assistant` 기본 채널이 실제 표시되는지
- 최근 6~12개월 `세션 소스/매체`에 저장된 AI 관련 도메인과 레거시 도메인
- Claude·ChatGPT·Gemini·Perplexity·Copilot의 웹·모바일 앱별 실제 리퍼러 전달 여부
- Search Console 생성형 AI 성과 보고서의 해당 속성 제공 여부와 현재 지원 지표
- Google Search Console 생성형 AI 보고서와 GA4 연결 보고서에서 공통으로 사용할 수 있는 페이지·기기·국가·날짜 범위
- 네이버 서치어드바이저 또는 분석 도구에 AI 브리핑·AI탭 전용 노출·클릭 구분값이 새로 제공되는지
- Search Analytics API를 `searchAppearance` 단독 차원으로 조회했을 때 해당 속성에서 생성형 AI 전용 값이 반환되는지
- Search Console 생성형 AI 보고서의 API·Bulk Export 정식 지원 여부
- 네이버 서치어드바이저 노출·클릭 보고서의 공개 API 또는 정식 내보내기 지원 여부
- 서버·CDN 로그 접근 가능 여부, 원본 리퍼러 저장 범위와 보유기간
- 견적·상담 폼에 최초 인지 경로 문항을 추가할 수 있는지
