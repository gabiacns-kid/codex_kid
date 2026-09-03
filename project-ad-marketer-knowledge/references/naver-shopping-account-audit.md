# Naver Shopping Search Account Audit And ADVoost Diagnosis

Use this reference when preparing a Naver Shopping Search Ads account review, diagnosing a shopping advertiser's account from user-provided notes, or writing a client-facing audit report where GabiaCNS has operation permission but Codex cannot access the ad account directly.

These notes are based on user-provided account review observations from a Toothnote Naver Ads account analysis on 2026-07-03. Treat platform controls as operational knowledge that should be checked in the live Naver ad account before final client commitment.

## 1. Newly Learned Facts

- Naver Shopping Search account reviews should separate "feature use exists" from "feature use is justified by enough data."
- Gender, age, and device bid modifiers can be useful, but early operation with thin data should usually start from a clean baseline.
- For a new or low-data account, setting all demographic/device weights to 100% for about one month can produce a more interpretable baseline before optimization.
- Excluded keywords should not be duplicated blindly at both ad group and material/product level. Group-level exclusions should cover common exclusions for all products in the group, while material/product-level exclusions should handle product-specific mismatch.
- This matters because excluded keyword registration limits can become a constraint as search-term matching expands.
- Partner/external media can dilute quality and performance for Shopping Search Ads; when efficiency matters, first restrict or evaluate partner media instead of running all inventory by default.
- Device importance is often easier to manage by PC/MO campaign separation than by device modifiers inside one campaign, because modifiers make actual CPC and rank interpretation less intuitive.
- Extension material should not be limited to review count or purchase count. Promotional text, sale-event copy, always-on USP, free shipping, or feature-led copy can be used to improve click motivation when eligible.
- Basic bid cleanup can be valuable before sophisticated bid strategy. A 70 KRW base-bid baseline can be used as a simple reset point before rank/product strategy is layered.
- Brand keywords and general keywords can be separated to prevent brand-keyword bid inflation and internal cannibalization.
- For shopping products, the ad-exposure product name can be used to test keyword coverage without changing the registered product name.

## 2. Corrections To Existing Naver Shopping Knowledge

- Do not praise demographic/device weighting simply because it is configured. Ask whether enough performance data exists to justify the modifier.
- Do not recommend all available products in a product family. Similar box counts, package sizes, or variants can split budget and blur judgment.
- Do not treat ADVoost as a default add-on for a limited-budget Shopping Search advertiser. If budget is constrained, stabilize Shopping Search first.
- Do not recommend ADVoost Boost Up before base ADVoost has enough learning and has already shown useful performance. Boost Up should be framed as a volume-expansion option after validation, not as initial setup.
- Do not describe ADVoost and Shopping Search as always synergistic. They can overlap in inventory or product demand and may split performance when budget is small.
- Do not rely only on ad account settings. Product competitiveness such as price, package, shipping, review, and product-page persuasion often explains poor conversion.

## 3. Practical Audit Principles

### Baseline Cleanup

For early or low-data Shopping Search accounts:

1. Reset gender, age, and device weights to 100% unless there is enough data showing obvious waste.
2. Rebuild excluded keyword logic:
   - group exclusions for all products in the group,
   - product/material exclusions for product-specific mismatch.
3. Review partner media exposure and restrict low-quality external inventory when efficiency is the main objective.
4. Split PC and mobile campaigns when device strategy matters.
5. Add extension copy for event and always-on selling points.
6. Reset base bids to a simple reference value, then adjust by rank, product role, and keyword intent.

### Product Selection

For multiple similar products in one product family:

- Do not operate every pack count or option.
- Select one representative product based on accessibility, margin, shipping benefit, price competitiveness, or review strength.
- Use the rest as non-ad, brand-only, or later test products unless there is a clear reason to split.

### Brand vs General Keywords

Use separate structures when brand search causes internal competition:

| Structure | Purpose |
|---|---|
| Brand keyword group | Defend self-brand demand and manage exposure order against external sellers |
| General keyword group | Acquire new shoppers by category or problem-intent keywords |
| Exclusion strategy | Prevent high-priority general products from wasting brand keyword budget or lower-priority products from cannibalizing |

### ADVoost Diagnosis

- ADVoost is a Naver automated performance display product that needs learning time after setup.
- Minimum learning period should be framed as 2+ weeks, with 4+ weeks preferable for judgment.
- If campaigns are paused or changed before the learning window, learning can be disrupted.
- For limited budgets, Shopping Search should usually be stabilized first.
- If later using ADVoost, consider excluding products already used heavily in Shopping Search or set a distinct role, such as target accumulation or discovery.
- Boost Up should be introduced only after base ADVoost has validated performance and the advertiser wants more volume.
- Boost Up may extend to verified external surfaces; therefore it should not be sold as guaranteed higher efficiency before base performance is checked.

## 4. Category And Product Examples From Toothnote

### Mouthwash

- Do not operate 1-box, 2-box, and 5-box products all at once without a reason.
- Choose one representative product:
  - 1 box for low entry price,
  - 2 boxes for margin/AOV balance,
  - 5 boxes for free-shipping or bundle benefit.
- If efficiency is the goal, avoid broad "mouthwash" only if it burns spend; focus on "disposable mouthwash" or similar feature-intent where the product's core differentiation is one-time use.

### Dental Floss

- Price competitiveness matters heavily because shoppers often compare value.
- If the product is less price-competitive than competitors, reduce budget share or hold the product.
- Be careful excluding very relevant terms such as Y-type floss while keeping only broader floss terms; broad terms may drive lower-intent traffic.
- Brand-keyword conversions can still justify a low-bid brand-defense structure.

### Whitening Gel

- High-CPC generic terms such as tooth whitening can produce purchases, but they may dominate budget.
- Separate objectives:
  - efficiency objective: reduce dependency on high-CPC generic keywords and test narrower alternatives,
  - acquisition objective: allocate a separate budget and evaluate with click volume, CVR, and new-user/upper-funnel metrics in addition to ROAS.
- If high-CPC keywords are retained, do not judge them only by short-term ROAS.

### Toothpaste

- Device modifiers can raise average CPC and make bid interpretation difficult.
- If PC/MO strategy differs, split campaigns and keep modifiers at 100%.
- If product names do not include functional terms, exposure may concentrate on generic "toothpaste."
- Use ad-exposure product names to test functional coverage where accurate:
  - whitening toothpaste,
  - fluoride toothpaste,
  - high-fluoride toothpaste,
  - gum toothpaste,
  - sensitive teeth toothpaste,
  - bad-breath toothpaste,
  - fluoride-free toothpaste,
  - tartar-control toothpaste.

## 5. Proposal And Report Wording

> 현재 계정은 쇼핑검색광고 운영 기능을 일부 활용하고 있으나, 데이터가 충분히 쌓이기 전 세부 가중치와 상품 동시 운영이 적용되어 효율 판단이 어려워질 수 있습니다. 초기에는 성별·연령·디바이스 가중치를 단순화하고, 상품군별 대표 상품을 중심으로 예산을 집중하는 것이 적합합니다.

> 제외키워드는 그룹과 소재에 동일하게 중복 등록하기보다, 공통 제외어는 그룹 단위에, 상품별로 다른 제외어는 소재 단위에 분리하는 구조가 좋습니다. 이렇게 해야 광고 운영이 누적되면서 제외키워드 등록 한도를 더 효율적으로 사용할 수 있습니다.

> 애드부스트는 네이버 AI가 노출 지면과 이용자 반응을 기반으로 운영하는 자동화 광고이므로 최소 2주, 가능하면 4주 이상 안정적인 학습 기간이 필요합니다. 예산이 제한적인 경우에는 쇼핑검색광고를 먼저 안정화한 뒤, 애드부스트는 타겟 축적 또는 추가 확장 목적에서 검토하는 것이 적합합니다.

> 부스트업은 애드부스트가 일정 수준 학습되고 성과가 확인된 뒤 더 많은 볼륨을 확보하기 위한 확장 옵션으로 보는 것이 안전합니다. 초기부터 부스트업을 적용하기보다 기본 애드부스트 성과를 먼저 확인한 뒤 적용 여부를 판단하는 방향을 권장드립니다.

> 가비아CNS는 네이버 쇼핑검색광고, 파워링크, 파워컨텐츠, 플레이스 광고에서 DIAD Pro를 활용해 순위별 최저 입찰가 확인, 최대 입찰가 관리, 시간대별 입찰 조정, CPC 효율 관리를 지원할 수 있습니다.

## 6. Items Requiring Confirmation

- Confirm the actual account's conversion volume by gender, age, device, media, product, and search term before applying modifiers.
- Confirm the live Naver excluded keyword limit and whether the limit applies separately by group and material/product in the current UI.
- Confirm partner media performance before blanket exclusion when the advertiser values reach or low CPC more than efficiency.
- Confirm actual ADVoost and Boost Up eligibility, external-surface scope, minimum budgets, and learning status in the current Naver Ads UI or official guide.
- Confirm product-level margin, shipping cost, review count, price competitiveness, and stock before selecting representative products.
- Confirm whether DIAD Pro settings can be applied to the specific product/ad type and account access level.

## 2026-08-27 변경 요약: 여행상품 계정의 대행사 비교와 전환 검증

### 1) 새로 학습한 사실

- 제공된 버디트립 리포트 합계에서 쇼핑검색광고는 광고비 5,857,312원, 클릭 10,474회, 구매 123건, 광고수익률 583%였고 파워링크는 광고비 7,402,251원, 클릭 8,069회, 구매 36건, 광고수익률 155%였다.
- 신규 운영 구간의 집행액은 기존 구간보다 매우 작아 두 대행사의 광고수익률 차이를 관리 역량 하나로 설명할 수 없었다. 기간, 예산, 판매상품 수, 랜딩페이지가 함께 달랐기 때문이다.
- 쇼핑검색 검색어 자료에서 구매수가 클릭수보다 많은 행이 확인됐다. 반복구매, 기여기간, 집계단위 또는 보고서 결합 방식의 영향일 수 있으므로 검색어 단위 극단적 광고수익률을 그대로 예산 확대 근거로 사용할 수 없다.

### 2) 기존 지식에서 수정할 점

- 대행사 변경 전후 성과를 비교할 때 광고비와 광고수익률만 제시하지 않는다. 동일 기간·상품·랜딩·전환 정의가 맞지 않으면 인과 판단을 보류한다.
- 여행상품의 구매 전환을 실제 이용 완료와 동일하게 보지 않는다. 결제 후 취소·변경·미이용 가능성을 반영해 최종 매출과 상담·예약 품질을 별도로 확인한다.
- 스마트스토어와 자사몰 중 한 곳을 일괄 우선하지 않는다. 즉시 결제형 상품은 스마트스토어, 일정·옵션 설명과 상담이 필요한 고관여 상품은 정보가 충분한 자사몰 또는 전용 랜딩으로 역할을 나눈다.

### 3) 실무 적용 원칙

1. 쇼핑검색과 파워링크를 동일 KPI로 단순 비교하지 않고 상품형 즉시구매 수요와 정보탐색·상담 수요로 역할을 구분한다.
2. 상품별 그룹, 검색 의도, 랜딩페이지, 제외 검색어를 연결해 구조를 재정리한다.
3. 초기 예산은 실제 구매 효율이 확인된 쇼핑검색에 우선 배정하고, 파워링크는 브랜드·구체 상품·일정·지역 등 고의도 검색어 중심으로 제한한다.
4. 검색어별 구매수가 클릭수보다 큰 경우 보고서 귀속기간, 직접·기여전환, 반복구매, 주문 취소 포함 여부를 먼저 확인한다.
5. 여행상품 KPI는 광고 결제뿐 아니라 실제 이용 완료 매출, 취소율, 상담 연결, 예약 확정까지 확장한다.

### 4) 제안서/리포트 문장 예시

> 제공 리포트에서는 쇼핑검색광고의 구매 효율이 파워링크보다 높게 나타났습니다. 다만 대행사 변경 전후의 기간·예산·상품 수·랜딩이 달라 성과 차이를 관리 역량 하나로 단정하기는 어렵습니다. 우선 상품별 검색 의도와 랜딩을 다시 연결하고, 동일한 전환 기준에서 쇼핑검색과 파워링크의 역할을 재검증하겠습니다.

> 일부 검색어는 클릭수보다 구매수가 크게 집계되어 전환 귀속 기준의 영향이 의심됩니다. 해당 수치를 바로 확대 근거로 사용하지 않고, 실제 이용 완료 매출과 취소율까지 확인한 뒤 예산을 조정하겠습니다.

### 5) 다음 확인 필요사항

- 각 대행사 운영 구간의 정확한 날짜, 일예산, 상품 수, 랜딩 URL
- 구매 전환의 귀속기간과 직접·기여전환 정의
- 결제 후 취소·변경·미이용을 제외한 실제 이용 완료 매출
- 상품별 마진, 현지 공급 가능 수량, 일정별 재고와 상담 처리 속도
