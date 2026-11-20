# Meta public-service traffic estimation

Use this reference when estimating Meta results for public information platforms, education programs, youth services, or other awareness-plus-traffic campaigns from recent in-house reports.

## 1. New facts and evidence boundaries

- Meta's Traffic objective can optimize for link clicks, landing-page views, or daily unique reach. When a website visit is the stated goal and Pixel measurement is available, prefer landing-page-view optimization and cost per landing-page view as the main KPI.
- Advertisers can include people under 18 based only on age and location. Do not propose interest, behavior, gender, lookalike, or retargeting logic for the 13-17 segment as if it were available in the same way as for adults.
- Facebook and Instagram have a minimum user age of 13. Under-13 audiences require guardian-, teacher-, or institution-facing communication rather than direct Meta targeting.
- A source report labelled only as `click` does not prove that the metric is a link click or a completed landing-page view.

Official references checked 2026-07-21:

- https://www.facebook.com/business/ads/ad-objectives/traffic
- https://www.facebook.com/help/980264326141711/
- https://www.facebook.com/help/messenger-app/717368264947302/

## 2. What to correct in existing estimation habits

- Do not average row-level CTR, CPC, or CPM values. Sum spend, impressions, and clicks first, then recalculate weighted metrics.
- Do not mix search, commerce conversion, event engagement, or foreign-currency reports into a public-service traffic benchmark without a comparability explanation.
- Deduplicate files and campaign totals before aggregation. A renamed copy with different file metadata can still contain the same performance totals.
- Do not calculate expected results from the gross proposal amount when VAT and agency fees are included.
- Do not label estimated clicks as site visits when landing-page-view history is missing.

## 3. Practical application rules

When the gross budget includes 10% VAT and a 15% agency fee on net media spend:

1. supply amount = gross budget / 1.1
2. net media spend = supply amount / 1.15
3. net agency fee = supply amount - net media spend
4. media amount including VAT = net media spend × 1.1
5. agency fee including VAT = gross budget - media amount including VAT

For comparable campaigns:

- weighted CTR = total clicks / total impressions
- weighted CPM = total net media spend / total impressions × 1,000
- weighted CPC = total net media spend / total clicks
- expected impressions = planned net media spend / weighted CPM × 1,000
- expected clicks = planned net media spend / weighted CPC

Use case-level minimum and maximum values as a visible planning range. Do not manufacture an independent best-case combination from the lowest CPM, highest CTR, and lowest CPC when those values came from different campaigns.

If awareness and traffic are both requested but the budget and creative count are limited, consider one Traffic campaign optimized for landing-page views. Manage reach, impressions, and frequency as secondary awareness KPIs. Split Awareness and Traffic into separate campaigns only when reach or frequency is a contractual primary KPI and each campaign has enough budget and creative volume.

## 4. Proposal and report wording

Prefer:

- "최근 유사 목적의 실집행 사례를 가중 합산해 기준 예상치를 산정했습니다."
- "예상 클릭은 첨부 리포트의 클릭 정의를 따른 값이며, 실제 사이트 방문은 랜딩페이지 조회로 별도 확인합니다."
- "총예산에서 VAT와 대행수수료를 분리한 순수 매체비를 기준으로 성과를 환산했습니다."
- "13-17세는 연령·위치 중심의 넓은 도달로 운영하고, 18세 이상과 보호자 대상에서만 계정에서 허용되는 세부 타겟팅을 검토합니다."
- 인지도와 트래픽 목적을 함께 운영할 때는 전액 트래픽 기준 클릭 수를 통합 성과로 제시하지 않는다. 전액 트래픽 클릭 수는 비교치로만 표시하고, 실제 운영안의 클릭 참고치는 트래픽 캠페인 배정 예산에만 CPC를 적용한다. 인지도 캠페인에서 부수적으로 발생하는 클릭은 사전 예상치에 합산하지 않는다.

Avoid:

- "클릭 = 방문"
- "13-17세 관심사 타겟팅"
- "총예산 전액이 매체비"
- "패션 전환 캠페인의 CTR을 공공 플랫폼 트래픽 예상치로 그대로 적용"

## 5. Next checks before launch

- Confirm whether the Meta Pixel can record landing-page views on the final URL.
- Add UTM parameters and verify GA4 or the site's analytics tool.
- Confirm whether the report's `click` field means link clicks, all clicks, or another result metric.
- Check the live account's estimated audience size after separating 13-17 and 18+ groups.
- Recheck current teen-ad restrictions and optimization options in Ads Manager immediately before launch.

## 2026-11-19 변경 요약: 공공·ESG 콘텐츠 전용관 트래픽과 연속형 소재 운영

### 1) 새로 학습한 사실

- 광고주가 `CRM 확보`라고 표현하더라도 실제 목표가 개인정보 수집이 아닌 전용관 방문과 콘텐츠 조회라면 CRM이 아니라 트래픽·콘텐츠 소비 KPI로 다시 정의해야 한다.
- 공공·ESG 전용관처럼 사업 소개, 사례, 영상, 신청 링크가 한 페이지에 모인 경우 1차 KPI는 전용관 랜딩페이지 조회로 둘 수 있다. 다만 페이지 조회만으로 개별 콘텐츠 소비를 증명할 수 없으므로 상세 콘텐츠 클릭, 영상 재생, 신청 링크 이동은 보조 행동 지표로 구분한다.
- 인스타툰은 정해진 공식 장수 규격이 있는 광고 단위가 아니다. 회차 수, 회차당 장수, 스토리보드·카피·수정 범위와 타 매체용 파생 소재를 견적에서 구분해야 한다.
- 서울시 사업처럼 사업 대상 지역이 고정된 경우 서울 지역 설정은 효율 선택이 아니라 적격성 조건이다. 다만 매체의 위치 정보는 이용자 위치·추정 거주지에 기반하므로 `서울 소재 기업 담당자만 정확히 노출`한다고 보장할 수 없다.

### 2) 기존 지식에서 수정할 점

- `CRM`을 단순 방문자 수나 콘텐츠 조회수의 동의어로 사용하지 않는다.
- 소재 2종을 2주 운영했다고 자동으로 통계적 우수 소재가 확정된다고 표현하지 않는다. 동일한 타깃·지면·예산·기간·랜딩 조건을 최대한 맞추고 데이터가 충분할 때 `상대 우수 소재`를 판단한다.
- 서울 지역 타겟팅만으로 서울 소재 기업을 식별한다고 설명하지 않는다. 지역 설정, 직무·관심군, `서울 소재 기업 대상`이라는 소재 문구를 함께 사용해 자기 선별을 유도한다.
- 인스타툰 원본을 카카오 비즈보드 등에 단순 리사이징할 수 있다고 전제하지 않는다. 매체별 정보량과 규격에 맞춘 별도 파생 소재가 필요하다.

### 3) 실무 적용 원칙

1. 1차 KPI는 랜딩페이지 조회수와 랜딩페이지 조회당 비용으로 두고, 도달·빈도·CTR·CPC는 진단 지표로 관리한다.
2. 초기 인스타툰 2편은 동일 조건에서 비교하며, 약 2주 후 충분한 데이터가 확보된 경우에만 상대 우수 소재의 예산 비중을 높인다.
3. 지속 운영 시 신규 회차를 기존 우수 소재와 비교하되, 빈도 상승과 반응 하락이 확인되면 기존 소재도 교체한다.
4. 제한 지역 사업은 지역을 확장하지 않는다. 타깃 확장은 서울 고정 상태에서 관심·직무 가설만 넓힌다.
5. 견적서에는 웹툰 편수·장수·기획·수정 횟수와 메타 캐러셀, 카카오 비즈보드·디스플레이 파생 소재 수량을 별도 항목으로 표시한다.

### 4) 제안서/리포트 문장 예시

> 본 캠페인은 사업 운영 범위를 고려하여 서울특별시를 필수 노출 지역으로 설정하고, 인사·채용, ESG·CSR, 사회공헌 및 경영지원 관심군을 중심으로 전용관 방문을 유도합니다. 초기 인스타툰 2편은 동일 조건에서 비교하며, 충분한 데이터가 확보된 경우 랜딩페이지 조회당 비용을 기준으로 상대 우수 소재의 운영 비중을 조정합니다.

### 5) 다음 확인 필요사항

- `서울 소재 기업`의 자격 기준과 소재에 표시해야 할 필수 문구
- 인스타툰 총 회차, 회차당 장수, 기획·카피·수정 포함 범위
- 제작비가 총예산에 포함되는지와 지속 운영 시 월별 신규 제작비
- 랜딩페이지 조회와 상세 콘텐츠 클릭·영상 재생·신청 링크 이동의 실제 측정 가능 여부
- 메타 광고계정의 최신 위치 옵션과 직무·관심 타겟 사용 가능 범위
