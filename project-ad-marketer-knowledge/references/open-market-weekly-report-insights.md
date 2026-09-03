# Open-Market Weekly Report Insight Pattern

Use this reference when reviewing or writing weekly performance comments for open-market ads such as Gmarket, Auction, 11st, eBay-style reports, Power Click-like products, keyword/product reports, and marketplace ROAS reports.

Source example:

- `ATWO_이베이&11번가_리포트 (1).pdf`, uploaded 2026-06-22.
- Report period shown in source: 2026-06-15 to 2026-06-21.

Treat this as a writing and analysis pattern, not a current performance benchmark.

## Core Comment Structure

Write comments in this order:

1. Market-level summary.
2. Per-market status: 11st, Gmarket, Auction, or other marketplace.
3. Cause interpretation: bid changes, weekday/weekend behavior, exposure/click decline, cost change, conversion status, ROAS movement.
4. Product-level observations: high-spend non-converting products, high-ROAS products, product groups needing bid/rank adjustment.
5. Keyword-level observations: high-spend non-converting keywords, conversion keywords, rank targets.
6. Concrete next actions with bid/rank numbers.
7. Previous action result.

Do not only say "performance declined" or "ROAS improved." Tie the statement to exposure, clicks, cost, conversions, revenue, and ROAS.

## Useful Thresholds From The Example

The report repeatedly uses these practical thresholds:

- `10,000원 이상 소진 + 미전환` as an action trigger for keyword/product bid reduction.
- `5,000원 이상 소진` as a threshold for Best/Worst product and keyword comparison tables.
- High-ROAS products and conversion keywords are candidates for rank/bid upward adjustment.
- Weekend bid reduction is evaluated by comparing weekday/weekend exposure, clicks, cost, revenue, and ROAS.

Use these thresholds as prior examples only. Adjust thresholds by advertiser budget, CPC, product price, and margin.

## Comment Patterns

### Market-Level Summary

Use:

```text
전 주 대비 전체적으로 성과가 하락했으며, 노출/클릭/비용이 함께 감소했습니다. 구매수는 증가했으나 구매금액은 감소하여 ROAS 개선 폭은 제한적입니다.
```

## 2026-07-09 Learning: Evidence-Gated Marketplace Report Validation

### 1. New Gmarket/Open-Market Applicable Inference

- Source: Codex thread `광고컨설팅(2)`, Toothnote Naver ad CSV validation and follow-up report work on 2026-07-09. The source media was Naver, but the validation logic applies directly to Gmarket/Auction/11st marketplace reports whenever exported report files and dashboard-only observations are mixed.
- When comparing a written insight with exported ad data, classify every claim before rewriting it:
  - `directly confirmed`: export contains the metric and the calculation can be reproduced.
  - `partially confirmed`: direction is supported, but exact wording or period must be adjusted.
  - `dashboard-only`: setting, rank, bid modifier, UI state, or competitive observation not present in the export.
  - `needs wording change`: the insight is directionally useful but overstates what the file proves.
- Separate total conversion from purchase-complete conversion. If the export contains multiple conversion types, do not say "conversion" as if all were purchase. Write purchase-complete and non-purchase conversion separately.
- If the same metric is evaluated across different periods, state the period every time. For example, a 7-day total and a post-restart 5-day total can support different conclusions.
- Keyword, placement, age, time, or product rows can support operating hypotheses, but do not infer hidden settings such as bid strategy, exact rank-control behavior, budget allocation intent, or platform-side automation settings unless the export or dashboard screenshot proves them.

### 2. Corrections To Existing Open-Market Report Practice

- Do not blend file-backed facts and dashboard-only judgment in one sentence. This makes the proposal sound stronger but weakens evidence discipline.
- For Gmarket AI Product Ads, this rule is more important because expanded keyword details and exact rank control may be unavailable or limited. Use keyword/contact-point data as diagnostic context, then make the action at product, product-cluster, campaign-type, bid/budget, or reporting level.
- In outbound or report emails, avoid saying "the data proves the campaign setting is wrong" when only exported performance is available. Better: "the export supports checking whether the current setting is still appropriate."
- For marketplace reports, product profitability, margin, stock, coupon/event participation, and hidden budget limits remain confirmation items unless explicitly provided.

### 3. Product-Centered Application Principles

- Before writing an action, ask what the export truly proves:
  1. Did spend occur?
  2. Did clicks occur?
  3. Did purchase-complete conversions occur?
  4. Is the trend period clear?
  5. Is the result tied to product, keyword, placement, time, device, or audience?
  6. Is the recommended action available in the current platform UI?
- For Gmarket/Auction after the AI Product Ads transition, translate file-backed findings into product-centered actions:
  - product to expand,
  - product to maintain,
  - product to observe,
  - product to reduce,
  - product detail/title/thumbnail to check,
  - campaign type to test,
  - report item to monitor next.
- When report data is thin, use `observe` or `test` wording instead of definitive scale/reduce recommendations.

### 4. Client-Facing Wording Examples

```text
이번 리포트에서 직접 확인되는 부분과 광고센터 화면에서 추가 확인이 필요한 부분을 나누어 보겠습니다. 파일상으로는 상품별 비용, 클릭, 구매완료 전환, ROAS 흐름은 확인 가능하지만, 실제 입찰 의도나 캠페인 설정값은 광고센터 화면 확인이 필요합니다.
```

```text
해당 상품은 클릭과 비용이 발생했지만 구매완료 전환은 확인되지 않았습니다. 다만 현재 리포트만으로 상품 경쟁력 문제인지, 노출 키워드/지면 문제인지, 입찰 강도 문제인지는 단정하기 어렵습니다. 우선 상품명, 대표 이미지, 가격/구성, 상세페이지 설득 요소를 함께 확인한 뒤 감액 또는 관찰 여부를 판단하는 것이 좋습니다.
```

```text
AI Product Ads에서는 키워드별 세부 통제가 제한될 수 있으므로, 키워드 데이터는 '어떤 수요와 접점이 있었는지'를 확인하는 용도로 보고 최종 운영 판단은 상품별 비용, 평균 CPC, 전환율, 전환매출, ROAS 기준으로 정리하는 것이 적합합니다.
```

### 5. Additional Verification Items

- Confirm whether the marketplace export contains purchase-complete conversion or all conversion types.
- Confirm whether bid/rank/age/time modifiers are included in the export or only visible in dashboard settings.
- Confirm current Gmarket AI Product Ads report fields before promising keyword-level, expanded-keyword, or exact-rank reporting.
- If the report is used for a seller-facing proposal, disclose the basis subtly: "리포트 기준", "광고센터 화면 기준", or "추가 확인 필요".

## 2026-06-29 Learning: 11st Beverage Weekly Report Email Pattern

### 1. Newly Learned Facts

- A 11st beverage weekly report can combine weekly trend, event/promotion effect, brand-keyword rank defense, AI campaign trend, and product addition proposal in one concise email.
- For Lingtea-style repeat-purchase beverages, weekly totals must be labeled by event context such as time deal or emergency supply. Event weeks should not be treated as ordinary baseline performance.
- AI campaign efficiency can decline even while total weekly sales recover through a promotion. This requires separate reading of promotion-supported sales and always-on AI efficiency.
- New products such as new flavor, sparkling, can, or package variants should be proposed as controlled test additions rather than mixed into all existing spend without a learning frame.

### 2. Corrections To Existing Knowledge

- Do not describe a weekly ROAS recovery as pure improvement if the week includes a timed deal or promotion.
- Do not treat AI recommendation performance and brand-keyword rank defense as the same operating task. Brand defense protects existing demand, while AI recommendation tests product expansion and recommendation-surface efficiency.
- If a coupon-support or boost program is proposed, explicitly mention discount-rate and margin risk before recommending participation.

### 3. Practical Application Principles

- Split the weekly reading into baseline, event, brand keyword, AI recommendation, and new-product test.
- For beverage products, compare flavor and format separately: zero peach, zero lemon-lime, recovery line, energy drink, sparkling, can/PET, multipack size.
- When event products produce purchases, identify whether one SKU carried the event result or whether multiple SKUs converted.
- When AI campaign ROAS falls below an internal threshold, first check which products consume cost without purchase before scaling or stopping the whole campaign.

### 4. Client-Facing Wording

```text
이번 주는 타임딜 영향으로 전주 대비 구매수와 구매금액은 회복되었으나, 전환율 자체가 큰 폭으로 개선되었다고 보기는 어렵습니다. 브랜드 키워드 순위 방어는 유지하되, AI 추천 영역에서는 효율 하락 상품과 신규 상품 테스트를 분리해 운영하는 것이 필요합니다.
```

```text
AI매출업 효율이 기준선 아래로 내려온 구간은 전체 캠페인 중단보다는 상품별 비용·구매·ROAS를 나누어 확인하는 것이 우선입니다. 신규 출시 상품은 기존 주력 상품과 같은 예산 안에서 섞기보다 별도 테스트 구간을 두어 클릭률과 구매 전환을 먼저 확인하는 방향을 제안드립니다.
```

### 5. Next Confirmation Items

- Confirm the margin and discount-risk range before participating in automatic coupon or boost programs.
- Confirm whether new products have enough stock, reviews, thumbnail readiness, price competitiveness, and promotion support before adding them to AI campaigns.
- Confirm whether weekly performance is being compared against a promotion week, non-promotion week, or stock/price-disrupted week.

Or:

```text
구매수는 소폭 감소했으나 매출액 증가로 수익률은 개선되었습니다. 일자별로 200% 이상 ROAS가 꾸준히 유지되어, 저효율 키워드 축소보다 고수익 키워드 순위 유지가 중요합니다.
```

### Bid Change Interpretation

Use:

```text
주말 입찰가 하향 조정 영향으로 주말 노출/클릭이 평일 대비 감소했습니다. 다만 주말 매출액이 유지되거나 더 큰 경우, 단순 하향보다는 전환 키워드와 미전환 키워드를 분리해 조정해야 합니다.
```

### High-Spend Non-Converting Keywords

Use:

```text
10,000원 이상 소진 키워드 중 미전환 키워드는 입찰가 또는 목표 순위를 하향 조정합니다.
```

Example action wording:

```text
KM385: 무선마우스키보드세트 1,500원 > 1,350원
플레이5: 무선헤드폰 1,400원 > 1,300원
E30T: 유선이어폰 1,020원 > 990원
```

### Conversion Keyword Rank Upward

Use:

```text
고수익률 상품의 전환 키워드는 순위 상향을 검토합니다. 단, 전체 상품 ROAS와 키워드별 CVR이 함께 확인된 경우에만 진행합니다.
```

Example action wording:

```text
포인트5: 무선게이밍마우스 3위 > 1위
AW111C: C타입이어폰 7위 > 5위
AW111C: 이어폰C타입 8위 > 6위
```

### Previous Action Result

Use:

```text
미전환 상품의 미전환 키워드 입찰가 및 순위 하향 조정, 고수익률 상품 키워드 상향 조정을 진행했습니다. 그 결과 수익률은 개선되었으나 노출/클릭/비용과 매출은 감소했습니다.
```

Add cause:

```text
주말 입찰가를 기존 대비 하향하면서 주말 노출과 클릭이 감소한 영향이 확인됩니다.
```

## Product/Keyword Classification

Classify rows as:

| Status | Signal | Action |
|---|---|---|
| Scale | High ROAS, conversion keyword exists, spend is controlled | Raise rank or bid gradually |
| Maintain | ROAS acceptable, conversions stable | Maintain current bid/rank |
| Reduce | Spend above threshold, no conversion, low ROAS | Lower bid or rank |
| Observe | Spend below threshold or data thin | Keep and review next week |
| Review product | Clicks exist but no purchase across multiple weeks | Check price, review, image, stock, benefit, product detail |

## Marketplace-Specific Cautions

### Gmarket/Auction

If the account reflects the 2026 product-centered operation environment, avoid overclaiming granular keyword control. Keyword/rank actions may still appear in old-style or report-based examples, but current recommendations should be adjusted to the actual UI:

- If keyword bid/rank control is available, use explicit keyword bid/rank actions.
- If only product-level bid strength is available, translate keyword findings into product-level bid strength adjustments.
- Use keyword data as search context when direct keyword exclusion or rank control is unavailable.

### 11st

Use product and keyword-level Best/Worst comparison when the report provides it. For high-spend non-converting items, propose bid/rank reduction and product competitiveness checks.

## Category-Specific Inference

Weekly marketplace interpretation must change by category.

- For beverages and repeat-purchase products, separate brand, category/function, flavor/variant, occasion, bundle, and promotion demand. Distinguish cost-control ROAS recovery from real sales growth.
- For seasonal fresh food, use a product lifecycle of prepare, enter, peak, late, exit, and evergreen. Always combine ad data with inventory, harvest, price, shipping, margin, and remaining sales-window information.
- The same product can perform differently by marketplace, campaign, placement, device, and promotion. Build a product-channel matrix instead of declaring an entire media channel efficient or inefficient from one weekly total.
- For detailed reasoning and client-facing examples, read `beverage-seasonal-fresh-food-marketplace-inference.md`.

## Client-Facing Weekly Comment Template

```text
전 주 대비 전체 노출과 클릭은 감소했으나, 구매수와 ROAS 흐름은 마켓별로 다르게 나타났습니다. 11번가는 비용과 매출이 함께 감소했고, 지마켓은 일부 고수익 상품에서 수익률 개선이 확인되었으나 전체 매출은 감소했습니다. 옥션은 구매수는 감소했지만 매출액 증가로 ROAS가 개선되었습니다.

차주에는 10,000원 이상 비용이 소진되었으나 전환이 없는 키워드/상품은 입찰가 또는 목표 순위를 하향 조정하고, 5,000원 이상 소진 구간에서 ROAS가 높은 상품과 전환 키워드는 순위 상향을 검토합니다. 단, 주말 입찰가 하향 이후 노출/클릭 감소가 확인되므로 주말 전체 입찰을 일괄 축소하기보다 전환 키워드와 미전환 키워드를 분리해 조정하는 방향이 적합합니다.
```
