# Naver Search, ADVoost, and Auto-Bidding Reference

## Powerlink Basics

Powerlink is keyword-based Naver search advertising. It is suitable for service and lead-generation advertisers when users actively search for a solution.

For education lead generation, do not judge success only by click or lead volume. Track:

- CTR
- CPC
- CVR
- CPL/CPA
- Consultation connection
- Reservation/visit
- Registration
- Revenue/ROAS if available

## Quality and Optimization Indicators

Naver search performance depends on relevance and expected click quality. Use indicators as operation triggers:

- Keyword and ad relevance
- Landing URL relevance
- Ad copy match
- Click expectation
- Conversion quality

If relevance is weak, review:

- Landing title/description and page content
- Mobile page quality
- Ad copy promise
- Keyword grouping
- Whether one URL is serving too many different intents

## ADVoost / Expanded Search

Treat ADVoost and expanded search as an operating environment, not an enemy.

Expanded search can expose ads to search terms not manually registered when the system judges the ad group, landing URL, and ad content relevant.

Operational rules:

1. Use expanded search to discover new intent.
2. Review search term reports regularly.
3. Classify terms into:
   - Promote to exact/controlled keyword
   - Observe
   - Add negative
   - Reflect in landing/content
4. Move high-value terms into controlled ad groups.
5. Match each intent to ad copy and landing.
6. Manage waste through negative keywords and grouping.

Proposal wording:

> 확장검색은 신규 검색어를 발견하는 탐색 장치로 활용하고, 검색어 리포트에서 성과 가능성이 확인된 검색어는 정식 키워드로 승격해 직접 관리하겠습니다. 승격 키워드는 별도 광고그룹 또는 기존 의도 그룹에 편입하여 입찰가, 소재, 랜딩 URL을 통제하고, 저효율 검색어는 제외 키워드로 관리해 확장성과 효율성을 동시에 확보하겠습니다.

## Match Type Logic

- Exact: registered keyword directly matches.
- Similar exact: close variant of registered keyword.
- Expanded: unregistered search terms can match based on ad/landing relevance.

Use exact/control for high-value terms; use expanded/search discovery with guardrails.

## Landing Readiness for AI-Based Matching

For Naver's AI expansion and relevance evaluation, landing pages should be crawlable and semantically clear.

Check:

- Page title clearly describes the page.
- Description summarizes the content.
- Main content is in text, not only image.
- Key benefits and course information are accessible in HTML.
- Mobile page is usable.
- No broken redirects, login walls, captcha, or blocked crawler.
- Each intent has the most relevant landing page.

## Daiad Pro / Auto-Bidding Differentiation

Use GabiaCNS's auto-bidding solution as a proposal differentiator.

Do not simply say "we maintain top rank." Stronger proposal:

- Segment keywords by role: main conversion, high CPC, brand defense, test/discovery.
- Test target positions by week or two-week periods.
- Compare CPC, CVR, CPA, ROAS by rank range.
- Find the most efficient position, not always #1.
- Use auto-bidding to maintain rank with minimum necessary bid.

Proposal wording:

> 가비아CNS는 단순 상위 노출이 아니라 키워드별 목표 순위와 수익성을 함께 검증합니다. 주요 전환 키워드, 고CPC 키워드, 고과금 키워드를 분류하고 주간 또는 격주 단위로 순위별 CPC·CVR·CPA·ROAS 변화를 비교해 가장 효율적인 노출 포지션을 찾겠습니다.

## Tracking Parameters

Naver search ads can use automatic tracking URL parameters and substitution variables.

Important parameters:

- `n_campaign_type`
- `n_ad_group`
- `n_media`
- `n_ad`
- `n_keyword`
- `n_keyword_id`
- `n_query`
- `n_match`
- `n_rank`
- `n_ad_group_type`

Important:

- `n_query` is the user's actual search query.
- `n_match` helps distinguish match type.
- Expanded search may not provide keyword id in the same way as registered keyword traffic.
- Always test landing URLs after adding parameters.

## 2026-07-10 Learning: ADVoost Max / Naver AI Briefing Ads

### 1. Source And Verification Status

- Official source checked on 2026-07-10: Naver Ads notice `네이버 AI 광고 출시 안내`, notice no. 31888, published 2026-06-15: https://ads.naver.com/notice/31888
- Additional source: user-provided Naver search ad operator notice pasted on 2026-07-10 describing ADVoost Max settings, insight report, disallowed industries, and reporting limits. Treat the pasted operator notice as user-provided current guidance unless the exact official notice URL is separately verified.

### 2. Officially Verified Facts From Notice 31888

- Naver AI ads start with `통합검색 > AI 브리핑`.
- Ad-center open date: 2026-07-15.
- Exposure open date: 2026-07-21.
- The official notice states the target product for formal service opening is `ADVoost 검색 광고`.
- AI Briefing ads appear only where Naver's ad agent judges ad exposure suitable.
- The ad is text-form and is intended to blend with AI Briefing content; format can change later.
- Ad copy is written by Naver's ad agent using advertiser-center and landing-page information; advertisers cannot directly edit that AI-written copy.
- AI ads can be controlled at ad-group registration/edit screens. At launch, ad groups using expanded search are set to ON by default.
- Targeting: time/day targeting is provided. Region, gender, age, and user segment targeting are used as hints for ad selection rather than deterministic selection controls.
- Billing is CPC. The CPC is based on the average Powerlink price related to the AI Briefing content, and a separate bid cannot be set.
- AI ads are exposed regardless of whether the advertiser registered the exact keyword. They use expanded-search budget, so the expanded-search budget cap must not be set too low if exposure is desired.
- Separate AI ad insight reporting is expected.
- Landing/advertiser readiness items:
  - schema.org fields such as `@type`, `name`, `description`, `price`, and `aggregateRating`;
  - readable site name in business channel information;
  - conversion script installation.
- The official notice says medical ad creatives subject to review may be restricted from AI Briefing exposure.
- AI ads can match all valid URLs in the ad group regardless of creative or keyword distinction.
- Final ad selection is handled by Naver's ad agent.

### 3. User-Provided Operator Guidance To Treat Carefully

The user's pasted operator guidance adds details that should be used with a source note until the exact official URL is confirmed:

- ADVoost Max is set in the existing expanded-search by ADVoost area at ad-group level.
- Ad groups using expanded search are ON by default at ad-center open; advertisers who do not want it should switch OFF.
- ADVoost Max performance appears in `검색광고 > 보고서 > ADVoost Max 인사이트`.
- Existing ad-management screens show only the total aggregate for ADVoost Max results.
- Targeting-level performance for region, gender, age, and user segments is not separately provided because those signals are only hints for ad selection.
- `내 광고 보기` can show where the AI agent exposed the ad and what AI-written ad text appeared, but not all AI-written texts are provided; it updates weekly on Monday when statistically meaningful.
- Pasted guidance lists disallowed industries as finance/insurance, health functional foods, and medical. This is broader than the official 31888 notice excerpt, which explicitly mentions medical-review restrictions. Verify before client delivery.
- Excluded keywords do not work for ADVoost Max because exposure is not directly matched to user search terms.
- ADVoost Max-specific performance is not separately provided in multidimensional/bulk reports beyond the ADVoost Max insight screen and aggregate totals in the basic ad-management screen.

### 4. Proposal And SEO/AEO Application

Use ADVoost Max as a conditional Naver expansion proposal when a Gmarket seller also appears to operate a self-owned mall or official site.

Positioning:

- ADVoost Max is not a classic manual keyword-rank product.
- It is closer to a context-matching AI search ad that uses AI Briefing context, ad-group/advertiser-center information, and landing-page content.
- Therefore, SEO/AEO readiness becomes part of paid-search readiness:
  - crawlable landing content,
  - schema.org product/local-business markup,
  - clear site name,
  - page title/description,
  - product/service description,
  - conversion script,
  - content that answers user exploration intent.

Client-facing wording:

```text
자사몰을 함께 운영 중이라면 G마켓 광고와 별도로 네이버 검색/AI 브리핑 영역까지 확장 검토가 가능합니다. ADVoost Max는 사용자가 직접 등록한 키워드에만 노출되는 구조가 아니라, 네이버 광고 에이전트가 AI 브리핑 문맥과 랜딩페이지 정보를 함께 판단해 광고를 선출하는 방식입니다. 따라서 단순 입찰가보다 사이트 이름, 랜딩페이지 설명, schema.org, 전환 스크립트 등 SEO/AEO 기반 점검이 중요합니다.
```

```text
다만 ADVoost Max는 별도 입찰가를 설정하는 상품이 아니며, 제외 검색어도 기존 검색광고처럼 작동하지 않습니다. 따라서 운영 전에는 자사몰의 랜딩 품질, 전환 추적, 업종 가능 여부, 확장검색 예산 비율을 먼저 점검한 뒤 테스트하는 것이 좋습니다.
```

### 5. Cautions Before Client Delivery

- Verify final ADVoost Max product name, eligibility, industry restrictions, report fields, and default ON behavior against current Naver official notices/help before formal proposal delivery.
- Do not propose ADVoost Max to restricted industries without confirmation. User-provided guidance says finance/insurance, health functional foods, and medical are unavailable; official notice 31888 explicitly mentions medical-review restrictions.
- Do not promise keyword-level control, negative-keyword exclusion, age/gender/location performance breakdown, or direct ad-copy editing.
- Because AI ad copy uses advertiser-center and landing-page information, poor site content can create weak or mismatched AI-generated messaging.

## 2026-07-30 update: ADVoost Max launch confirmation

### 1) 새로 학습한 사실

- Naver's official 2026-07-08 notice confirmed the ADVoost Max advertiser-center opening on 2026-07-15 and ad serving opening on 2026-07-21.
- ADVoost Max is controlled at ad-group level within the existing `확장검색 by ADVoost` setting. Ad groups already using expanded search were scheduled to default to ON at advertiser-center opening.
- AI Briefing performance is checked in `검색광고 > 보고서 > ADVoost Max 인사이트`. The basic ad-management screen shows aggregate ADVoost Max results, while region, gender, age, and user-segment performance is not separately supplied because those settings act as ad-selection hints.
- Official source checked 2026-07-30: https://ads.naver.com/notice/32709

### 2) 기존 지식에서 수정할 점

- The uploaded August media report says the AI agent rewrites copy and `결정 가격을 성과에 맞춰` 운영한다고 요약했지만, client wording should remain more precise: advertisers cannot set a separate ADVoost Max bid, and CPC is determined by Naver's stated ADVoost Max pricing logic rather than by a freely editable AI bid.
- Do not describe demographic/location settings as strict exclusion or guaranteed targeting controls for ADVoost Max. They are hints and do not produce a separate targeting-level report.
- Do not leave the default ON setting unchecked during account takeover. Review every expanded-search ad group before spending begins.

### 3) 실무 적용 원칙

1. Audit all expanded-search ad groups for ADVoost Max ON/OFF status.
2. Check landing-page text, business information, schema, conversion scripts, and all URLs inside the ad group because AI-written copy and URL selection rely on account and landing information.
3. Use the dedicated ADVoost Max Insight report and compare it with the aggregate management-screen figure.
4. If control, report granularity, or industry eligibility is insufficient, keep ADVoost Max OFF for that ad group and test only after prerequisites are corrected.

### 4) 제안서/리포트 문장 예시

> ADVoost Max는 AI 브리핑 문맥과 랜딩페이지 정보를 바탕으로 광고 문안과 연결 대상을 판단하는 확장형 검색광고입니다. 기존 확장검색 광고그룹은 기본 ON 여부를 먼저 점검하고, 전용 인사이트 보고서에서 실제 노출 문안과 성과를 확인한 뒤 유지 여부를 결정하겠습니다.

### 5) 다음 확인 필요사항

- Current restricted-industry list and account-level eligibility.
- Final pricing description and any later changes to CPC calculation.
- Whether insight-report fields, update frequency, or targeting hints change after launch stabilization.

## 2026-09-04 변경 요약: 파워링크 기본 소재와 확장소재를 실제 노출 형태로 제안하는 기준

### 1) 새로 학습한 사실

- 네이버 공식 도움말 기준 파워링크 기본 소재의 제목은 15자 이내, 설명은 20~45자로 작성한다.
- 추가제목은 광고그룹 단위로 15자 이내에서 등록할 수 있으며, 단일형 기본 소재와 함께 노출되는 확장소재다.
- 파워링크 이미지와 서브링크도 기본 소재의 주목도와 이동 경로를 보완하는 확장소재로 등록할 수 있다.
- 확장소재는 등록과 심사를 완료해도 검색 위치와 광고 성과 등에 따라 노출 여부와 조합이 달라질 수 있다. 따라서 제안서의 소재 예시는 실제 등록 가능한 구성으로 만들되 동일한 화면 노출을 보장하는 표현은 쓰지 않는다.
- 공식 출처 확인일: 2026-09-04.
  - 기본 소재 글자 수: https://ads.naver.com/help/faq/1480
  - 확장소재 종류와 노출 조건: https://ads.naver.com/help/faq/1134

### 2) 기존 지식에서 수정할 점

- `제목 예시·설명 예시·랜딩`만 나열한 일반 표는 광고주가 실제 노출 모습을 판단하기 어렵다. 가능하면 `업체명 → 노출 URL → 제목·추가제목 → 설명 → 이미지 → 서브링크` 순서로 광고 화면에 가까운 예시를 보여준다.
- 상품 장점을 많이 넣기 위해 제목을 길게 작성하지 않는다. 제목은 브랜드와 상품군을 담백하게 식별하고, 구체적인 기능과 선택 이유는 추가제목과 설명에 나눠 배치한다.
- 가격, 할인율, 배송, 재고, 사은품처럼 변하는 정보는 랜딩페이지와 집행 시점에 확인된 경우에만 사용한다. `1위`, `최고`, `완벽`, `절대 안전`처럼 객관적 입증이나 심의가 필요한 표현은 근거 없이 넣지 않는다.
- 제품 안전 기능은 절대적 결과로 확대하지 않는다. 예를 들어 전도 시 물샘 방지 구조는 `물이 새지 않는다`가 아니라 `전도 시 물샘을 줄이는 구조`로 표현한다.

### 3) 실무 적용 원칙

1. 광고그룹의 검색 의도와 랜딩 상품을 먼저 정한 뒤 제목, 추가제목, 설명, 이미지, 서브링크를 한 세트로 설계한다.
2. 제목에는 브랜드·상품군, 추가제목에는 핵심 기능·용량, 설명에는 차별점과 확인 행동을 배치한다.
3. 서브링크는 용량별 모델, 기능 안내, 세척 방법, 관련 상품군처럼 기본 랜딩을 보완하는 경로로 구성한다.
4. 이미지와 문구의 상품이 동일한지, 서브링크가 정상 페이지로 연결되는지, 모바일과 PC에서 잘리는 표현이 없는지 집행 전에 확인한다.
5. 품절 또는 재입고 예정 상품은 판매 재개와 가격을 확인한 뒤 활성화하고, 품절 기간에는 예산을 판매 가능한 우선 상품으로 이동한다.
6. 소재 제안서에는 제목·추가제목·설명의 실제 글자 수를 함께 표시해 등록 가능성을 사전에 검토한다.

### 4) 제안서/리포트 문장 예시

> 파워링크 소재는 업체명, 노출 URL, 제목·추가제목, 설명, 이미지, 서브링크까지 실제 노출 순서에 맞춰 구성합니다. 제목에는 브랜드와 상품군을 짧게 제시하고, 설명에는 상세페이지에서 확인되는 제품 특징과 공식몰에서 확인해야 할 이유를 담습니다. 확장소재는 등록하더라도 노출 위치와 광고 성과에 따라 실제 표시 조합이 달라질 수 있습니다.

> 재고와 가격이 수시로 바뀌는 상품은 집행 직전 랜딩페이지를 확인한 뒤 광고를 활성화합니다. 품절 상태에서는 같은 상품군 광고를 무리하게 유지하지 않고 판매 가능한 상품으로 예산을 이동합니다.

### 5) 다음 확인 필요사항

- 계정의 소재 유형이 단일형인지 반응형인지와 추가제목 사용 가능 여부.
- PC·모바일별 실제 확장소재 조합과 노출 빈도.
- 이미지 및 서브링크 심사 결과, 랜딩 URL 정상 작동 여부.
- 집행 직전 상품 재고·가격·프로모션과 광고 문구의 일치 여부.

## 2026-09-15 변경 요약: ADVoost 플레이스 Beta·TV맛집 노출·첫 광고비 지원

### 1) 새로 학습한 사실

- `ADVoost 플레이스(Beta)`는 2026년 9월 16일 오후 광고주센터에서 먼저 제공될 예정이다. 업체와 하루 예산을 정하면 클릭 수 최대화를 목표로 입찰가를 실시간 조정하고, 지역·성별·연령·매체 등을 별도로 설정하지 않은 채 자동 타겟팅하며, 스마트플레이스의 이미지와 혜택 정보로 소재를 자동 구성한다.
- 신규 플레이스 광고그룹 생성 시 `ADVoost 플레이스 자동 운영`이 기본 선택된다. 기존 그룹에는 자동 적용되지 않는다. 자동 운영에서는 입찰가·지역·성별·연령·매체와 자동 생성 소재를 직접 수정할 수 없지만 요일·시간대는 직접 정할 수 있다.
- ADVoost 플레이스는 CPC 방식이며 플레이스 페이지 이동뿐 아니라 전화, 예약, 저장하기, 길찾기, 방문자 리뷰, 플레이스 플러스 등 광고 요소 클릭에도 과금된다. 하루 예산이 전액 소진될 수 있고, 업체 이미지가 최소 1개 필요하며 병·의원 업종은 이용할 수 없다.
- 2026년 9월 17일부터 음식점 플레이스광고는 PC·모바일 통합검색, 모바일 플레이스·지도 앱, PC 지도검색에서 `흑백요리사맛집`, `TV에나온맛집` 같은 TV맛집 관련 검색어와 `TV에나온` 필터 결과에 노출될 수 있다. 기존 등록 방법과 랭킹 기준은 유지된다.
- 2026년 5월 7일 이후 첫 광고비 지원은 광고주센터 가입일부터 60일 안에 광고주가 직접 신청해야 한다. 해당 기간의 유상 광고비만 합산해 최대 50만 원의 무상 비즈쿠폰을 지급하며 사업자등록번호·광고주센터 로그인 ID 기준 1회다. 광고주센터에서 집행하는 명시 대상 상품만 포함되고 NOSP 구매 상품은 제외된다.
- 공식 출처 확인일: 2026-09-15.
  - https://ads.naver.com/notice/34109
  - https://ads.naver.com/notice/34145
  - https://ads.naver.com/notice/30385

### 2) 기존 지식에서 수정할 점

- ADVoost 플레이스를 수동 플레이스광고의 단순 자동입찰 기능으로 설명하지 않는다. 자동 타겟팅과 자동 소재까지 묶인 별도 운영 방식이며 직접 통제 범위가 줄어든다.
- 신규 그룹의 기본 선택 상태를 그대로 두지 않는다. 지역 제한, 매체 선택, 소재 문구 통제가 중요한 광고주는 수동 운영이 더 적합할 수 있다.
- 클릭 수 최대화를 방문·예약 성과 최적화로 표현하지 않는다. 전화·길찾기·저장하기 등 과금 클릭 이후의 실제 방문과 매출은 별도로 확인해야 한다.
- TV맛집 관련 노출을 모든 음식점의 자동 노출 또는 방송 출연 인증으로 설명하지 않는다. 관련 검색어·필터에서 조건에 부합하는 광고가 노출될 수 있다는 범위로 제한한다.
- 첫 광고비 지원을 자동 지급이나 현금 환급으로 설명하지 않는다. 가입일 기준 신청 기한, 유상 광고비, 대상 상품, 1회 제한과 환불 불가 비즈쿠폰 조건을 먼저 확인한다.

### 3) 실무 적용 원칙

1. 플레이스 광고그룹 생성·인수 시 자동 운영과 수동 운영 중 무엇이 선택됐는지 확인한다.
2. 지역·연령·매체·소재 통제가 중요하면 수동 운영을 우선하고, 넓은 자동 탐색이 목적이면 별도 예산의 ADVoost 플레이스 Beta 테스트를 고려한다.
3. ADVoost 플레이스 평가는 클릭 수뿐 아니라 전화 연결, 예약 완료, 길찾기 후 방문, 쿠폰 사용, 매출 등 후속 지표로 보완한다.
4. 스마트플레이스의 대표 이미지, 혜택, 영업시간과 휴무 정보를 광고 입력값으로 보고 집행 전 정비한다.
5. 신규 광고주는 계정 가입일과 첫 광고비 지원 신청 가능 여부를 온보딩 첫날 확인하고, 지원금은 미디어 예산의 확정 재원으로 선반영하지 않는다.

### 4) 제안서/리포트 문장 예시

> ADVoost 플레이스는 입찰가뿐 아니라 타겟과 소재까지 자동 운영하는 Beta 기능입니다. 지역과 소재를 세밀하게 통제해야 하는 매장은 기존 수동 운영을 유지하고, 자동 탐색이 필요한 매장은 별도 예산으로 비교 테스트하겠습니다.

> 플레이스 광고의 과금 클릭에는 상세페이지 이동 외 전화·예약·저장·길찾기 등이 포함됩니다. 클릭 수 증가만으로 방문 성과를 판단하지 않고 예약 완료와 실제 방문에 가까운 행동을 함께 확인하겠습니다.

> 첫 광고비 지원은 대상 광고주가 가입일부터 60일 안에 직접 신청해야 하며, 유상 광고비 범위에서 최대 50만 원의 광고용 비즈쿠폰으로 지급됩니다. 계정의 가입일과 기존 수혜 이력을 확인한 뒤 적용 가능 여부를 안내드리겠습니다.

### 5) 다음 확인 필요사항

- 2026년 9월 16일 ADVoost 플레이스 Beta 실제 오픈 여부와 계정별 제공 범위
- 스마트플레이스센터 순차 적용 일정과 Beta 종료 후 기능·보고서 변경
- 자동 운영과 수동 운영의 동일 조건 비교 및 실제 방문·예약 성과
- TV맛집 관련 질의·필터의 광고 노출 조건과 해당 음식점의 자격 정보
- 첫 광고비 지원 신청 화면 노출, 가입일, 대상 상품, 기존 수혜 이력

## 2026-09-15 변경 요약: 파워링크 URL 치환 변수와 소액 예산 계정 구조

### 1) 새로 학습한 사실

- 파워링크 연결 URL 또는 추적 경유 URL에 `{keyword}`, `{query}`, `{ad}` 등의 예약어를 넣으면 광고 클릭 시 각각 등록 키워드, 실제 검색어, 소재 ID로 치환된다. URL 치환 변수에는 별도의 ON/OFF 설정이 없으며 연결 URL에 사용하면 작동한다.
- 캠페인의 자동 추적 URL 파라미터를 활성화하면 `n_keyword`, `n_query`, `n_ad`, `n_match` 등이 별도로 추가된다. `{keyword}`는 확장검색으로 확장된 검색어에서 제공되지 않을 수 있으므로 실제 검색어 확인은 `n_query`와 검색어 보고서를 함께 사용한다.
- 같은 광고그룹의 키워드가 동일 랜딩페이지를 사용한다면 그룹 공통 URL에 `utm_term={keyword}&utm_content={ad}`를 넣어 키워드와 클릭 소재를 함께 식별할 수 있다. `{ad}` 결과는 사람이 읽는 소재명이 아니라 `nad-...` 형태의 소재 ID다.
- 공식 출처 확인일: 2026-09-15.
  - https://ads.naver.com/help/faq/1335

### 2) 기존 지식에서 수정할 점

- 키워드별 성과 추적을 위해 모든 키워드에 고정 UTM URL을 각각 작성해야 한다고 설명하지 않는다. 랜딩이 같으면 치환 변수가 포함된 공통 URL로 운영을 단순화할 수 있다.
- `utm_content={ad}`를 소재명 자동 입력으로 표현하지 않는다. 소재 ID와 실제 소재명·소구 방향을 연결하는 별도 매핑표가 필요하다.
- `utm_term={query}`를 기본값으로 권장하지 않는다. 광고계정의 등록 키워드 성과는 `{keyword}`, 실제 검색어 탐색은 `n_query` 또는 검색어 보고서로 구분한다.

### 3) 실무 적용 원칙

1. 상품군별로 랜딩페이지가 같으면 그룹 공통 URL에 `utm_source=naver`, `utm_medium=cpc`, 캠페인 규격, `utm_term={keyword}`, `utm_content={ad}`를 설정한다.
2. 소재 ID와 관리용 소재명·소구·버전을 별도 시트에서 매핑한다.
3. PC와 모바일의 노출 구좌와 목표 순위가 다르면 캠페인을 디바이스별로 분리하고, 상품군과 키워드 유형을 광고그룹으로 나눈다.
4. 소액 예산에서는 일반·대표 키워드 그룹에만 일예산을 걸고 브랜드·세부 키워드는 개별 최대입찰가와 순위로 통제한다.
5. URL 파라미터 추가 후 랜딩 정상 작동, 파라미터 유지, GA4 수집을 실제 클릭 전 테스트한다.

### 4) 제안서/리포트 문장 예시

> 동일 상품군의 키워드는 공통 랜딩 URL에 네이버 치환 변수를 적용해 등록 키워드와 클릭 소재를 함께 구분합니다. 소재값은 광고 ID로 수집되므로 별도 소재 관리표와 연결해 소구별 성과를 확인합니다.

> PC와 모바일은 노출 구좌가 달라 캠페인을 분리하고, 브랜드 키워드는 상위 노출, 일반·대표 키워드는 1페이지 중간 순위를 초기 기준으로 운영합니다. 소액 테스트에서는 과금이 집중되는 일반 그룹에만 일예산을 적용합니다.

### 5) 다음 확인 필요사항

- 실제 계정의 그룹 공통 연결 URL 적용 위치와 키워드 개별 URL의 우선순위
- 확장검색 클릭에서 `{keyword}` 공란 처리와 GA4 표기 방식
- 카페24 리디렉션 과정의 UTM 및 네이버 자동 추적 파라미터 유지 여부
- 소재 ID와 확장소재 ID가 실제 보고서에서 구분되는 범위
