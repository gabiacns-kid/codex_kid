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

## 2026-09-07 변경 요약: 쇼핑검색광고·ADVoost 쇼핑 노출 위치 및 개수 동적 최적화 확대

### 1) 새로 학습한 사실

- 네이버 공식 공지 기준, 2026년 9월 10일부터 쇼핑성 질의가 노출되는 `네이버 통합검색 PC`, `네이버 쇼핑 모바일`, `네이버 쇼핑 PC`에도 이용자 반응에 따라 키워드별 광고 노출 구성을 실시간 최적화하는 방식이 도입될 예정이다.
- 이 방식은 기존 `네이버 통합검색 모바일`에 적용되던 최적화 범위를 추가 지면으로 확대하는 내용이다.
- 광고·일반·슈퍼적립 상품의 위치와 개수는 고정되거나 보장되지 않고 최적화 결과에 따라 동적으로 달라질 수 있다.
- 이번 공지는 쇼핑검색결과의 노출 구성 변경이며, 광고 등록 방법·노출 순위 산정·과금 방식은 기존 쇼핑검색광고 운영과 동일하다고 안내됐다.
- 공지일은 2026년 9월 3일이며 적용 예정일은 2026년 9월 10일이다. 일정은 내부 사정에 따라 바뀔 수 있다.
- 공식 출처 확인일: 2026-09-07. https://ads.naver.com/notice/34004

### 2) 기존 지식에서 수정할 점

- `지면 확대`를 광고 슬롯 수가 항상 증가하거나 광고 노출 기회가 일률적으로 늘어나는 변화로 설명하지 않는다. 확대되는 것은 동적 최적화의 적용 지면이며 실제 광고 위치·개수는 질의와 이용자 반응에 따라 달라진다.
- 특정 시점의 PC·모바일 검색 화면에서 확인한 광고 순위와 개수를 계정의 고정 노출 상태로 표현하지 않는다.
- 적용 전후 성과가 달라져도 원인을 이번 노출 구성 변경 하나로 단정하지 않는다. 입찰가, 상품 경쟁력, 경쟁 광고, 수요, 프로모션과 재고를 함께 본다.
- 광고 위치가 유동적이라는 이유로 기존 입찰·순위 관리가 무의미해졌다고 해석하지 않는다. 순위 산정과 과금 방식은 기존과 동일하다는 공식 안내 범위 안에서 운영한다.

### 3) 실무 적용 원칙

1. 2026년 9월 10일 전후 보고서는 적용 전·후 기간을 구분하고, PC 통합검색과 네이버쇼핑 PC·모바일 성과를 지면·기기별로 비교한다.
2. 단일 노출진단 화면보다 노출수, 클릭수, 평균 CPC, 전환수, 매출, 광고수익률의 기간 추이를 우선한다.
3. 노출 위치와 개수 변화가 의심될 때는 동일 키워드·유사 시간대의 반복 확인과 실제 계정 지표를 교차 검토한다.
4. 상품별 노출 감소가 확인되면 입찰가만 올리기 전에 가격, 배송, 리뷰, 재고, 상품명과 대표 이미지 등 경쟁력을 함께 점검한다.
5. 쇼핑검색광고와 ADVoost 쇼핑을 함께 운영할 때는 상품·지면별 직접 전환과 비용 변화를 분리해 확인하고, 동적 노출을 성과 보장 근거로 사용하지 않는다.

### 4) 제안서/리포트 문장 예시

> 네이버는 2026년 9월 10일부터 통합검색 PC와 네이버쇼핑 PC·모바일에서도 이용자 반응에 따라 광고 위치와 개수를 유동적으로 구성할 예정입니다. 특정 순위의 고정 노출을 전제로 운영하기보다 상품별 노출·클릭·전환 추이를 지면과 기기별로 확인하고 예산과 입찰을 조정하겠습니다.

> 이번 변경은 광고 등록, 순위 산정, 과금 방식의 개편이 아니라 노출 구성 최적화의 적용 지면 확대입니다. 광고 개수가 항상 늘어나는 것으로 해석하지 않고 적용 전후의 실제 계정 데이터를 기준으로 영향 여부를 판단하겠습니다.

### 5) 다음 확인 필요사항

- 2026년 9월 10일 실제 적용 여부와 이후 일정 변경 공지
- 광고주 계정에서 지면·기기별 노출수, 클릭률, CPC, 전환율 변화
- 네이버가 공개하는 최적화 판단 신호의 추가 안내 여부
- 쇼핑검색광고와 ADVoost 쇼핑 상품별 보고서에서 동적 노출 영향을 구분할 수 있는 세부 항목

## 2026-09-15 변경 요약: 쇼핑 컬렉션·네이버 메인 쇼핑지면 재편과 테스트 구분

### 1) 새로 학습한 사실

- 2026년 9월 3일부터 모바일 통합검색 일부 질의의 가격비교와 네이버플러스 스토어 컬렉션이 단일 쇼핑 컬렉션으로 통합됐다. 쇼핑검색광고 위치와 개수는 트래픽에 따라 달라질 수 있고, 브랜드스토어 상품 광고 블록과 네이버플러스 스토어 고평점 리뷰 상품 광고 블록은 검색어·블록 우선순위에 따라 통합 컬렉션 하단에 가변적으로 노출될 수 있다.
- 트렌드뷰형 상품카드에서는 컬러칩이 추가되고 `추가 홍보 문구`는 삭제됐다. 리뷰·구매·찜 수와 가격 표시 UI도 변경됐다. 상품 클릭 후에는 클릭 상품과 비교할 연관 상품 추천 영역이 노출될 수 있다.
- 네이버는 2026년 9월 11~17일 모바일 통합검색 일부 트래픽에서 개선 쇼핑 컬렉션을 테스트한다. 인기상품 탭은 최대 4페이지, 인기 브랜드·카테고리·시리즈 탭은 페이지당 광고 최대 6개가 노출될 수 있고, 복수 트렌드 탭은 `요즘 트렌드` 단일 탭으로 합쳐질 수 있다. 이는 테스트 조건이며 상시 노출 보장이 아니다.
- 2026년 9월 16일부터 네이버 PC 메인 쇼핑블록의 비로그인 `지금뜨는` 영역이 대분류 추천 광고를 보여주는 `카테고리픽`과 베스트차트 기반 `지금뜨는` 탭으로 분리될 예정이다. `네이버 메인-PC` 매체 설정이 ON이어야 노출 후보가 된다.
- 2026년 10월 12일부터 네이버 메인 모바일 쇼핑판의 기존 트렌드Pick 보장형 광고가 종료되고, 해당 블록에 쇼핑검색광고 쇼핑몰상품형과 ADVoost 쇼핑이 노출될 예정이다. 로그인 이용자는 구매이력 유무에 따라 함께 구매할 상품 또는 인기 상품, 비로그인 이용자는 슈퍼적립·슈퍼특가 등 프로모션 추천 광고가 노출될 수 있다. `네이버 메인-모바일` 매체 설정이 ON이어야 한다.
- 네이버는 2026년 9월 17~24일 모바일 통합검색 일부 트래픽에서 쇼핑 컬렉션의 전체 상품 수까지 검색어별 이용자 반응에 따라 바꾸는 테스트를 진행할 예정이다. 광고 위치·개수 최적화와 컬렉션 전체 길이 최적화는 구분해야 한다.
- 네이버가 공개한 ADVoost 쇼핑·부스트 업 사례에서 부스트 업을 15일 이상 운영한 계정의 평균 구매 ROAS 약 560%, 일부 업종의 네이버 지면 대비 최대 1.4배 수치가 소개됐고 일 예산 5만 원 이상이 운영 팁으로 제시됐다. 공식 공지도 이 수치가 개별 계정 기록이며 평균 또는 보장 성과가 아니라고 명시한다.
- 공식 출처 확인일: 2026-09-15.
  - https://ads.naver.com/notice/33795
  - https://ads.naver.com/notice/33965
  - https://ads.naver.com/notice/34104
  - https://ads.naver.com/notice/34090
  - https://ads.naver.com/notice/34091
  - https://ads.naver.com/notice/34093

### 2) 기존 지식에서 수정할 점

- `지면 확대`를 모든 상품의 노출량 증가로 설명하지 않는다. 매체 설정이 ON이어도 추천·검색어·이용자 반응에 따라 노출되지 않을 수 있다.
- 9월의 쇼핑 컬렉션 테스트 결과를 정식 운영 규칙으로 사용하지 않는다. 테스트 기간, 일부 트래픽, 적용 예정 공지를 각각 표시한다.
- 추가 홍보 문구가 보이지 않는 트렌드뷰형 지면에서는 문구 확장보다 대표 이미지, 가격·혜택, 리뷰 신뢰, 상품명 매칭이 더 중요해질 수 있다. 다만 모든 쇼핑 지면에서 추가 홍보 문구가 폐지된 것으로 확대 해석하지 않는다.
- 네이버 사례의 ROAS 560%와 최대 1.4배를 제안서의 예상 성과나 업종 기준값으로 사용하지 않는다. 계정별 상품 구성, 외부 매체 연동, 예산, 운영기간과 집계기준이 달라 재현을 보장할 수 없다.
- 부스트 업 일 예산 5만 원은 네이버의 운영 권장값이지 모든 광고주에게 적합한 최소 예산이나 성과 보장 조건이 아니다. 월예산과 기존 쇼핑검색·ADVoost 쇼핑 예산을 함께 보고 집행 가능성을 판단한다.

### 3) 실무 적용 원칙

1. 9월 3일, 9월 16일, 10월 12일을 기준으로 통합검색 모바일·PC 메인·모바일 쇼핑판 성과를 구분해 비교한다.
2. 계정 인수 시 `네이버 메인-PC`, `네이버 메인-모바일` 매체 ON/OFF를 확인하고, 원치 않는 확장 노출을 막거나 지면 테스트 목적을 명확히 한다.
3. 컬렉션 UI 변화 이후 대표 이미지별 CTR, 할인·혜택 표시, 리뷰·구매 신호, 상품별 CVR을 함께 확인한다.
4. 쇼핑검색광고, ADVoost 쇼핑, 부스트 업은 상품과 목적을 분리하고 각 캠페인의 직접 전환·비용·신규 도달을 따로 판단한다.
5. 테스트 공지 기간에는 단일 시점 노출진단보다 일자·기기·지면별 추이를 기록하고 테스트 종료 후 정식 적용 공지를 다시 확인한다.

### 4) 제안서/리포트 문장 예시

> 네이버 쇼핑광고는 통합검색과 메인 쇼핑판에서 추천형 노출을 확대하고 있습니다. 다만 매체를 켠다고 모든 상품의 노출이 늘어나는 구조는 아니므로, PC·모바일 메인 지면을 별도 확인하고 상품별 클릭률과 전환율을 기준으로 유지 여부를 판단하겠습니다.

> 모바일 통합검색 일부 트래픽에서는 쇼핑 컬렉션의 구성과 전체 상품 수를 유동적으로 조정하는 테스트가 진행됩니다. 테스트 기간의 순위나 광고 개수를 고정 기준으로 사용하지 않고, 적용 전후의 노출·클릭·전환 추이를 비교하겠습니다.

> 네이버가 소개한 부스트 업 성과는 개별 광고계정 사례이므로 예상 ROAS로 제시하지 않습니다. 기존 쇼핑검색광고와 ADVoost 쇼핑의 상품별 성과를 먼저 확인한 뒤, 월예산 안에서 외부 매체 확장이 가능한 경우에 한해 별도 테스트하겠습니다.

### 5) 다음 확인 필요사항

- 2026년 9월 16일 PC `카테고리픽` 탭 실제 적용 여부와 일정 변경
- 2026년 9월 17~24일 컬렉션 길이 테스트 종료 후 정식 적용 여부
- 2026년 10월 12일 모바일 쇼핑판 전환과 트렌드Pick 보장형 종료 여부
- 계정별 네이버 메인 PC·모바일 매체 성과와 ADVoost 쇼핑·부스트 업 상품 중복
- 컬렉션 UI별 `추가 홍보 문구` 노출 범위와 광고 보고서의 세부 지면 구분 가능 여부

## 2026-10-06 변경 요약: 도서 카탈로그형 스토어의 ADVoost 쇼핑 운영 기준

### 1) 새로 학습한 사실

- ADVoost 쇼핑은 네이버 쇼핑에 입점한 몰의 전체 상품을 연동하고, AI가 상품 선정·타겟·입찰·예산·노출 지면을 실시간으로 최적화한다.
- 전체 상품이 연동 대상이어도 모든 상품의 균등 노출은 보장되지 않는다. 실제 노출은 구매 가능성과 지면별 성과 예측에 따라 선별된다.
- 운영 단위는 광고그룹·소재가 아닌 애셋그룹이며, 아이템 세트로 특정 카테고리와 상품을 포함하거나 제외할 수 있다. 네이버는 가능하면 `모든 아이템`을 포함하는 구성을 권장한다.
- 스마트스토어는 비즈채널 등록 시 전환 추적이 자동 신청된다. 캠페인은 `전환 가치 최대화` 입찰 전략을 사용하며 실시간 구매 전환을 기반으로 학습한다.
- 상품명·이미지는 네이버 쇼핑 등록 정보를 그대로 사용하며 광고용으로 별도 수정할 수 없다. 상품 정보 변경은 최대 1시간, 초기 연동과 최적화는 최대 48시간이 소요될 수 있다.
- 2026년 9월 30일부터 모바일 웹 카페 홈 피드에, 10월 7일부터 카페 앱 홈 피드에 ADVoost 쇼핑이 추가 노출될 예정이다. 일정은 변경될 수 있다.
- 공식 출처 확인일: 2026-10-06.
  - https://ads.naver.com/help/faq/1361
  - https://ads.naver.com/help/faq/1372
  - https://ads.naver.com/help/faq/1374
  - https://ads.naver.com/notice/31988
  - https://ads.naver.com/notice/34386

### 2) 기존 지식에서 수정할 점

- `전 상품 노출`을 모든 상품이 균등하게 노출된다는 뜻으로 사용하지 않는다. `전체 상품을 학습·선정 대상으로 연동`한다고 표현한다.
- 도서 제목이 검색어와 맞는다는 이유만으로 자동화 광고의 성과를 단정하지 않는다. 동일 도서 가격, 할인·적립, 배송, 출고 가능 여부, 리뷰와 시리즈 묶음 구성이 전환 선별에 영향을 줄 수 있다.
- 애셋그룹을 도서 1권당 세분화하지 않는다. 전체 카탈로그를 학습시키되, 판단이 필요한 경우에만 아동·학습, 전집·세트, 일반 단행본 등 의미 있는 상품군으로 구분한다.

### 3) 실무 적용 원칙

1. 초기에는 모든 판매 가능 도서를 포함한 1개 애셋그룹으로 시작해 학습 모수를 확보한다.
2. 품절·판매 중단·정보 불일치 상품을 정리하고, 상품명·표지 이미지·세트 구성·출고 조건을 광고 시작 전에 점검한다.
3. 최소 2주, 가능하면 4주 이상 큰 설정 변경 없이 운영하고 상품 성과 보고서에서 노출·클릭·구매·매출·ROAS를 도서별로 확인한다.
4. 예산이 제한적이면 일반 쇼핑검색광고와 ADVoost 쇼핑을 동시에 과도하게 확장하지 않고, ADVoost 쇼핑의 전 상품 자동 선별 기능을 먼저 테스트한다.
5. 부스트 업은 네이버 외부 매체 확장 옵션으로, 기본 ADVoost 쇼핑의 상품별 성과와 예산 소진 안정성이 확인된 뒤 별도로 테스트한다.

### 4) 제안서/리포트 문장 예시

> 내꿈은어부는 특정 도서 하나를 키워드별로 직접 운영하는 방식보다, 스토어의 전체 도서 카탈로그를 광고 학습 대상으로 연동하는 ADVoost 쇼핑이 운영 특성에 더 잘 맞습니다. AI가 도서명·카테고리·상품 정보와 이용자의 구매 가능성을 함께 판단해 노출 상품과 지면, 입찰가, 예산을 자동 최적화하도록 운영합니다.

> 초기에는 판매 가능한 도서 전체를 포함해 학습 범위를 넓히고, 최소 2~4주간 큰 설정 변경 없이 상품별 성과를 확인합니다. 이후 구매·매출·ROAS와 예산 소진 현황을 기준으로 상품군 분리 여부와 부스트 업 확장을 판단합니다.

### 5) 다음 확인 필요사항

- 스토어의 실제 판매 중 상품 수, 품절·판매 중단 상품, 카테고리별 상품 비중
- 최근 30일 주문·매출·전환 규모와 일 예산으로 학습이 가능한지
- 일반 단행본, 전집·세트, 학습지·교육도서의 주문당 광고비 허용 차이
- 도서 할인·적립, 배송비, 출고 가능 여부와 상품 정보 정합성
- 부스트 업 사용 자격과 외부 매체 연동 여부
