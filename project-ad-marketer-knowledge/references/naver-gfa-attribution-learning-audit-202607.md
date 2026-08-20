# Naver GFA Attribution and Learning Audit

Reviewed: 2026-07-24

Use this reference when diagnosing Naver display/GFA accounts that show strong CTR or CPC but weak ROAS, frequent budget or creative changes, heavy Brand Search revenue concentration, or a gap between last-click and data-based contribution conversions.

## 1. Confirmed Current Facts

### Contribution conversion

- Naver contribution conversion combines Search Ads and Display Ads rather than evaluating them as separate media.
- `기여전환(마지막클릭)` gives 100% credit to the final ad click before conversion.
- `기여전환(데이터기반)` distributes fractional credit across multiple ad clicks using Naver's data-based model.
- These metrics are provided at campaign level in `전체 캠페인`.
- They are Beta metrics. Naver states that the aggregation standard may change.
- They are available from 2026-03-23 data onward.
- The default conversion tracking window is 15 days and can be set from 7 to 20 days.
- `총 전환` and contribution conversions are not directly interchangeable. Total conversions separate Search and Display and use last click within each ad type, so one user journey can be counted once in each ad type. Contribution conversion integrates the two ad types.

Official sources:

- https://ads.naver.com/help/faq/1461
- https://ads.naver.com/help/faq/1215
- https://ads.naver.com/help/faq/1460

### Learning and change history

- For Display Ads using conversion value maximization, Naver states that targeting or creative changes, large budget or bid-cap changes, and long ad-group pauses can reset learning and reduce efficiency.
- Do not say every budget edit resets learning. First identify whether the change was large, whether creative or targeting changed, whether the group was paused, and whether the UI actually shows a learning-state change.
- Naver recommends, specifically for conversion value maximization, keeping an ad group to five or fewer creatives.
- For conversion value maximization, Naver states that approximately 30 valid purchase-complete conversions with conversion value within one week are needed for optimization.

Official source:

- https://ads.naver.com/help/faq/821

### Own-mall audience options

- A non-Smart Store advertiser cannot use Smart Store/Brand Store event audiences as `스토어 타겟`.
- This does not mean own-mall advertisers have no advanced audience options.
- When web conversion tracking is installed, collected conversion data can support website audiences and conversion optimization.
- Own-mall and external-mall advertisers can use ADVoost Audience after registering web conversion tracking, subject to live account eligibility and sufficient data.
- Before saying remarketing or advanced targeting is impossible, check the website-audience list, audience size, event coverage, lookback window, and whether the target is usable.

Official sources:

- https://ads.naver.com/help/faq/845
- https://ads.naver.com/help/faq/848
- https://ads.naver.com/help/faq/924

## 2. Diagnostic Interpretation Rules

### High CTR and low ROAS

Do not conclude that users clicked and left because the price was surprising. That is one hypothesis only.

Other plausible causes:

- broad or low-intent audience delivery;
- promotion-led creative that earns clicks without building purchase intent;
- landing-message mismatch;
- mobile usability, page speed, checkout, or payment friction;
- weak review and trust evidence;
- product-option or shipping friction;
- tracking gaps or duplicated/missing purchase events;
- audience expansion quality;
- creative fatigue or accidental clicks by placement.

Required evidence:

`Impression -> Click -> Session -> Engaged session -> View item -> Add to cart -> Begin checkout -> Purchase -> Revenue`

Break this funnel down by campaign, ad group, creative, landing page, device, and UTM.

### Data-based contribution is slightly higher than last click

A positive difference means the campaign received additional multi-touch credit. It does not, by itself, prove brand lift or profitable assistance.

Always calculate:

1. additional attributed conversions and revenue;
2. percentage lift versus last click;
3. data-based attributed revenue divided by spend;
4. change in revenue share, not only conversion count;
5. whether extra credit is concentrated in low-value events.

If conversion count rises more than attributed revenue, the additional credit may be concentrated in lower-value conversions. Do not use the count increase alone to justify budget.

### Brand Search revenue concentration

High Brand Search revenue concentration confirms that conversion is concentrated in high-intent branded traffic. It does not prove loyalty, satisfaction, or that Display Ads created the demand.

Possible demand sources include:

- existing customers;
- offline retail;
- marketplace exposure;
- PR, influencer, social, or earned media;
- organic search;
- Display Ads;
- seasonality or stock changes.

To claim assisted brand demand, compare:

- branded query volume and Brand Search clicks over time;
- direct and organic brand sessions;
- GFA reach and spend with an agreed lag;
- exposed versus non-exposed or holdout results when possible;
- GA4 assisted paths and Naver contribution metrics together.

Brand Search reports often show no variable media cost because Brand Search is a contract product. Add the actual contract fee and contract period before calculating ROAS or reallocating budget.

## 3. Audit Checklist

Before proposing a new GFA structure, obtain:

1. Identical date ranges for Search, Display, and GA4.
2. GFA campaign, ad-group, creative, placement, device, gender, and age reports.
3. Purchase-complete count and revenue, not only total conversions.
4. Bid strategy, optimization event, learning status, CBO status, budget, bid cap, and frequency settings.
5. Creative start date and material change date.
6. Naver conversion window and GA4 attribution settings.
7. GA4 ecommerce funnel by UTM campaign/content and landing page.
8. Purchase event deduplication, order ID, payment-domain, and cross-domain tracking QA.
9. Brand Search contract fee, keyword group, contract period, and renewal history.
10. Product margin, allowable CPA, break-even ROAS, refunds, cancellations, and stock.

## 4. Client-facing Wording

> 데이터기반 기여전환에서 GFA의 보조 기여가 확인되더라도, 증가 폭과 비용 대비 기여매출을 함께 확인해야 합니다. 따라서 GFA를 단순 중단하거나 반대로 브랜딩 효과로 과대평가하지 않고, 동일 기간의 브랜드 검색량·GA4 구매 여정·소재별 성과를 결합해 역할과 예산을 재정의합니다.

> 자사몰은 네이버 스토어 타겟을 사용할 수 없지만, 웹 전환 추적 데이터를 활용한 웹사이트 타겟과 자동 오디언스 활용 가능성은 남아 있습니다. 실제 사용 가능 여부는 현재 모수와 이벤트 수집 상태를 확인한 뒤 결정합니다.

> 높은 클릭률과 낮은 광고수익률만으로 가격이 이탈 원인이라고 단정할 수 없습니다. 소재가 만든 기대와 상품페이지의 정보, 결제 편의성, 후기, 실제 구매 단계의 이탈을 순서대로 확인해 원인을 분리하겠습니다.

## 2026-07-24 Update — Conversion-event composition and contract-cost normalization

### 1) 새로 학습한 사실

- 웹사이트 전환 캠페인의 `전환 수 최대화`는 캠페인에서 선택한 최적화 전환 유형을 기준으로 동작한다. 최적화 전환 유형은 `모든 전환`, `장바구니 담기`, `구매 완료` 중 하나이므로, 입찰 전략 이름만으로 구매 완료 최적화라고 판단하면 안 된다.
- 네이버는 웹사이트 전환 광고 최적화에 최근 1주 이내 전환 40회가 필요하다고 안내한다. 광고 그룹 설정·소재 변경, 큰 폭의 예산 또는 입찰가 한도 변경, 장시간 OFF는 재학습을 유발할 수 있다.
- 조지루시 사례의 2026-05-01~07-22 GFA 기기 보고서에서는 총 전환 284건 중 구매 완료 7건, 장바구니 담기 277건이었다. 이 수치는 `총 전환수`가 실질 구매성과를 대표하지 않을 수 있음을 보여주는 파일 기반 사례다.
- 브랜드검색은 계약형 상품이므로 보고서의 광고비가 0원이어도 무비용 매출로 해석하면 안 된다. 현재 계약비는 계약 일수로 일할 환산한 뒤 같은 기간 매출과 비교해야 한다.

공식 출처:

- https://ads.naver.com/help/faq/1377

사례 근거:

- `기기데이터_result.csv` (2026-05-01~2026-07-22)
- `계약 목록 20260724 1018.xlsx`

### 2) 기존 지식에서 수정할 점

- `전환 수 최대화`를 곧바로 구매 최적화로 표현하지 않는다. 반드시 캠페인 화면의 `최적화 전환 유형`을 별도로 확인한다.
- 총 전환당비용이 낮더라도 총 전환 대부분이 장바구니라면 구매 CPA·구매 CVR·구매 ROAS를 우선 평가한다.
- 브랜드검색 매출 비중이 높다는 사실만으로 브랜드검색 효율이 높다고 표현하지 않는다. 계약비, 계약기간, 상품유형 변경일을 결합해야 한다.
- 전환 가치 최대화의 `광고 그룹당 소재 5개 이하` 권장은 전환 수 최대화에 그대로 확정 적용하지 않는다. 전환 수 최대화에서는 공식 도움말의 “소재를 너무 많이 운영하면 학습이 원활하지 않을 수 있음” 범위로 표현한다.

### 3) 실무 적용 원칙

1. `총 전환수 = 구매완료 + 장바구니 + 기타 전환`으로 분해하고 구매 비중을 계산한다.
2. 최적화 전환 유형이 모든 전환 또는 장바구니라면 낮은 전환당비용이 구매 최적화의 증거가 아님을 명시한다.
3. 구매완료 전환이 적으면 성별·연령별 구매 1~2건을 근거로 타겟을 즉시 축소하지 않는다. 우선 소재·랜딩·결제·후기 가설을 검증한다.
4. 브랜드검색 계약이 갱신되거나 상품 유형이 바뀐 날을 기준으로 이전/이후 성과를 분리한다.
5. 계약 목록의 기간과 계약명이 충돌하면 계약비 환산을 확정하지 않고 광고주센터 계약 상세 화면에서 재확인한다.

### 4) 제안서/리포트 문장 예시

> 보고서상 총 전환은 발생하고 있으나 대부분이 장바구니 담기에 집중되어 있어, 현재 성과를 구매 전환 성과로 해석하기 어렵습니다. 캠페인의 최적화 전환 유형을 확인한 뒤 구매 완료 중심으로 운영 목표와 평가 지표를 재정렬하겠습니다.

> 브랜드검색의 매출 비중은 높지만 계약형 상품의 고정비가 일반 보고서 광고비에 반영되지 않을 수 있습니다. 계약기간별 비용을 일할 환산하여 실질 광고수익률을 다시 산출한 뒤 예산 배분을 결정하겠습니다.

### 5) 다음 확인 필요사항

- 현재 텀블러 캠페인의 최적화 전환 유형이 `모든 전환`, `장바구니 담기`, `구매 완료` 중 무엇인지.
- 최근 1주 기준으로 해당 최적화 전환이 40회 이상 안정적으로 발생하는지.
- 브랜드검색 계약 목록의 PC 프리미엄 계약기간과 계약명에 표시된 기간이 다른 이유.
- 월 1,000만 원 예산에 브랜드검색 계약비가 포함되는지 별도인지.

## 2026-07-24 Update — External conversion hypotheses and Brand Search keyword pruning

### 1) 새로 학습한 사실

- 조지루시 GFA 캠페인의 최적화 전환 유형은 `모든 전환`으로 확인되었다. 총 전환 284건 중 구매 완료 7건, 장바구니 담기 277건이므로 자동 입찰이 학습하는 전환 대부분이 장바구니인 사례다.
- 조지루시 공식몰의 다수 상품 상세페이지에서 `사용후기 0`이 확인된다. 리뷰 부재는 관찰 가능한 사실이지만, 구매 전환 저하의 원인이라는 판단은 검증 가설로 구분해야 한다.
- 2026-05-01~07-23 브랜드검색 검색어 보고서에서 가습기 관련 키워드는 모바일 노출 11,955회, 클릭 1,621회였으나 직접·간접 전환과 구매매출이 모두 0이었다.
- 2026 브랜드검색 프로모션 단가표 기준 모바일 라이트형은 30일·VAT 제외 기준 `8,001~15,700회 170만 원`, `15,701~22,100회 260만 원`이다. 구간 하향이 실제 재견적에서 확인될 경우 월 90만 원(VAT 제외)의 차이가 발생한다.

공식 출처:

- https://ads.naver.com/help/faq/1377
- https://ads.naver.com/help/faq/1290
- https://ads.naver.com/help/faq/1055

사례 근거:

- `계정 보고서,1957990 (3).csv` (2026-05-01~2026-07-23)
- `naver_brandsearch_price_2026.xlsx`
- 조지루시 공식몰 상품 상세페이지

### 2) 기존 지식에서 수정할 점

- 가격, 브랜드 인지도, 리뷰 부족 같은 광고 외 요인을 제안서에서 무조건 제외하지 않는다. 관찰 사실과 추론을 분리하고 `전환 저하 가능 요인` 또는 `검증 가설`로 제시한다.
- 프로모션 소재가 클릭 접근성을 높인다고 해서 구매 설득까지 해결한다고 보지 않는다. 할인·증정 소재와 품질·내구성·서비스·사용후기 등 구매 확신 소재를 구분해 운영한다.
- 구매 표본이 적을 때 연령·성별 전환 1~2건을 근거로 즉시 타겟을 축소하지 않는다. 명백히 부적합한 범위만 제한하고 구매완료 데이터가 쌓인 뒤 재조정한다.
- 브랜드검색에서 전환 없는 키워드를 삭제한다고 계약비가 자동으로 줄어드는 것은 아니다. 키워드 정보 확인 화면에서 그룹 검색수 합계와 예상 견적이 실제로 하위 구간으로 내려가는지 확인해야 한다.

### 3) 실무 적용 원칙

1. GFA 저성과는 `입찰·타겟·소재`와 `가격·리뷰·결제·재고·상세페이지`를 함께 진단하되, 원인 확정과 가능성 진술을 분리한다.
2. 모든 전환 최적화에서 장바구니가 대부분이면 구매완료 중심 KPI를 별도로 관리하고, 구매완료 전환량이 학습 조건에 부족하다는 제약도 함께 밝힌다.
3. 리뷰가 없으면 후기 적립금, 체험단·오프라인 구매자 후기 이관 가능성, 이미지·영상 UGC 사용권, 리뷰 모듈 노출 위치를 광고 외 개선안으로 제안한다.
4. 품절 상품 브랜드 키워드는 직접·간접 전환과 교차 구매가 없으면 다음 계약에서 제외하는 것을 우선 검토한다. 재입고 일정이 확정되면 재입고 전 수요 회수용 키워드로 복원한다.
5. 브랜드검색 비용 절감액은 `현재 그룹 검색수 합계 - 제외 키워드 검색수`를 광고주센터에서 다시 조회하고 실제 단가 구간이 바뀔 때만 확정한다.
6. 이미 집행 중인 계약의 비용을 줄이려면 단순 키워드 OFF가 아니라 계약 취소·재계약 여부와 환급 예상액을 확인한다.

### 4) 제안서/리포트 문장 예시

> 장바구니까지의 관심은 형성되고 있으나 구매완료 전환은 제한적입니다. 가격대와 브랜드 친숙도, 공식몰 상품후기 부족은 구매 확신 단계의 이탈을 설명할 수 있는 요인으로 판단되며, 결제 편의성·배송·상품정보와 함께 순차적으로 검증하겠습니다.

> 현재 가습기 관련 브랜드 키워드는 검색 수요는 있으나 품절 상태에서 직접·간접 전환이 확인되지 않았습니다. 다음 계약에서는 해당 키워드를 제외한 그룹 검색수와 예상 견적을 다시 산정하고, 실제 단가 구간이 낮아질 경우 절감 예산을 GFA 인지도 및 구매 설득 소재에 재배분하겠습니다.

### 5) 다음 확인 필요사항

- 가습기 키워드를 제외했을 때 광고주센터 `키워드 정보 확인`에 표시되는 모바일 그룹 검색수 합계와 예상 견적.
- 현재 계약을 중도 취소·재계약할 경우 실제 환급액과 최소 과금액.
- 가습기 재입고 예상일과 재입고 알림·예약구매 전환 경로 제공 가능 여부.
- 후기 적립금, 외부 후기 사용권, 오프라인 구매자 리뷰 수집 가능 여부.

## 2026-08-20 Update — 월 100만 원 GFA의 단일 목표 운영과 예상치 제시 원칙

### 1) 새로 학습한 사실

- 제공된 7월 타 업종 GFA 데이터에서 인지도·트래픽 캠페인 합계는 광고비 1,357,590원, 노출 650,066회, 클릭 2,754회, 평균 CPC 약 493원, 구매전환율 0.25%, 광고수익률 10.93%였다.
- 같은 자료의 웹사이트 전환 캠페인 합계는 광고비 2,313,187원, 노출 147,115회, 클릭 1,567회, 평균 CPC 약 1,476원, 구매전환율 3.57%, 광고수익률 79.97%였다.
- 전환 캠페인 내부에서 체험형 상품과 본품의 구매 효율 차이가 컸다. 목적별 평균만으로 새 광고주의 구매성과를 보장할 수 없으며 상품 가격·혜택·상세페이지의 영향을 분리해야 한다.
- 현재 네이버 도움말 기준 인지도 및 트래픽 캠페인은 웹사이트·앱 방문과 클릭 확대가 목적이며 최적화 전환 유형은 제공하지 않는다.

공식 확인:

- 네이버 광고주센터 `인지도 및 트래픽 광고는 무엇인지 궁금해요.` 최종 수정일 2026-06-22, 확인일 2026-08-20: https://ads.naver.com/help/faq/1366
- 네이버 광고주센터 `인지도 및 트래픽 광고는 어떻게 만드나요?` 최종 수정일 2026-06-22, 확인일 2026-08-20: https://ads.naver.com/help/faq/1371

### 2) 기존 지식에서 수정할 점

- 월 100만 원에서 트래픽과 전환 캠페인을 기계적으로 나누지 않는다. 새 카테고리 교육이 우선이면 첫 달은 트래픽 한 가지 목표로 충분한 소재 표본을 확보한다.
- 타 업종·타 상품 성과를 동일 업종 평균이나 보장 수치로 표현하지 않는다. `제공된 캠페인 데이터를 예산에 환산한 참고 범위`로 표시한다.
- 트래픽 목적의 구매수와 광고수익률은 보조 지표이며 주된 평가는 클릭·CTR·CPC·상세페이지 유입이다.
- 체험형 상품의 전환성과 상단값을 본품에 그대로 적용하지 않는다.

### 3) 실무 적용 원칙

1. 월 100만 원은 1캠페인·1광고그룹·소재 3~4개를 기본으로 시작한다.
2. 새로운 필요성을 설명하는 상품은 문제 인식, 기존 습관 점검, 사용 루틴, 신뢰·혜택 소재로 역할을 나눈다.
3. 최소 7일 관찰 후 한 번에 한 요소만 변경하고, 잦은 예산·타겟·소재 변경을 피한다.
4. 예상 수치는 CPC·CPM·CTR 관측 범위와 산식, 상품 판매가를 함께 제시한다.
5. `노출 대비 클릭 저조` 또는 `클릭은 높지만 구매행동·CVR 저조`를 소재·랜딩 교체 기준으로 통일한다.
6. 전환 캠페인은 구매완료 수집, 최근 구매 신호, 허용 CPA, 손익분기 광고수익률이 확인된 뒤 검토한다.

### 4) 제안서/리포트 문장 예시

> 월 100만 원은 트래픽과 전환 목표를 동시에 충분히 학습시키기 어려운 규모입니다. 첫 달은 인지도·트래픽 캠페인에서 어떤 메시지가 상세페이지 방문을 만드는지 확인하고, 구매 신호와 손익 기준이 확보되면 전환 캠페인을 별도 월에 검증하겠습니다.

> 아래 수치는 동일 업종 평균이 아니라 제공된 7월 캠페인 데이터를 월 예산에 환산한 참고 범위입니다. 실제 성과는 소재, 상품 가격, 상세페이지, 타겟과 계절 수요에 따라 달라질 수 있습니다.

### 5) 다음 확인 필요사항

- 광고계정의 스마트스토어 구매완료 전환 수집 상태
- 최근 7일 구매완료·장바구니 전환량과 최적화 가능 여부
- 상품별 원가율, 허용 CPA, 손익분기 광고수익률
- 지면별 CPC·CTR·구매행동과 파트너 매체 포함 여부
- 첫 달 상위 소재의 메시지와 전환 캠페인 승계 기준
