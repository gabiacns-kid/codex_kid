# Beverage And Seasonal Fresh-Food Marketplace Inference

Use this reference when analyzing weekly marketplace reports for beverages, hydration products, repeat-purchase consumer goods, seasonal fruit, fresh food, seafood, meat, regional specialties, or sellers whose active products change with harvest and inventory.

Sources learned on 2026-06-25:

- `링티 11번가 0621 주간리포트 전달드립니다` email, report period 2026-06-15 to 2026-06-21.
- `링티 이베이 260621 주간리포트 전달드립니다` email.
- `삼다몰 26.06월 3주차 광고 집행 및 변경 사항 전달드립니다` email, major comparison period 2026-06-16 to 2026-06-22.

Treat these as operating examples, not universal performance benchmarks.

## 1. Reasoning Sequence

Do not jump from `ROAS moved` directly to `raise or lower the bid`.

Use this sequence:

1. **Describe the metric movement**
   - exposure, clicks, CPC, cost, purchases, revenue, CVR, AOV, and ROAS.
2. **Decompose the movement**
   - traffic effect, conversion-rate effect, order-value effect, or cost-control effect.
3. **Check the intervention**
   - bid, budget, product inclusion, product exclusion, promotion, time deal, emergency supply, placement, or campaign-type change.
4. **Check the demand environment**
   - season, weather, payday or month opening, event period, harvest, inventory, competitor promotion, delivery deadline, or platform traffic.
5. **Check product and channel fit**
   - the same product can perform differently by marketplace, campaign type, device, placement, and search context.
6. **Choose the next test**
   - maintain, concentrate, expand, reduce, stop, or prepare the next seasonal product.
7. **State the confidence level**
   - confirmed by data, plausible hypothesis, or requires additional data.

## 2. Critical Interpretation Rules

### ROAS Improvement Is Not Always Growth

- If cost falls faster than revenue, ROAS can improve while the business becomes smaller.
- Call this `efficiency defense` or `cost-control recovery`, not `sales growth`.
- A healthy scale-up requires revenue or contribution profit to grow while ROAS remains above the acceptable threshold.

### ROAS Decline Is Not Always Failure

- If cost and purchases increase but revenue is flat, inspect AOV and product mix.
- A lower-priced product entering the sales mix can lower ROAS even when order volume improves.
- During a launch or peak-season capture period, temporary ROAS decline can be acceptable only when margin, inventory, and customer value support it.

### Promotion Weeks Need A Separate Baseline

- Time deals, emergency promotions, coupons, and platform events should not be compared directly with ordinary weeks as if the media conditions were identical.
- Compare:
  1. normal week versus normal week;
  2. promotion versus similar promotion;
  3. promotion-day result versus surrounding days.

### One-Week Zero Conversion Is Not A Universal Stop Rule

- Stop quickly when spend is material relative to product margin and purchase frequency.
- Observe longer when the denominator is small, CPC is low, or purchase timing is irregular.
- Use a spend threshold tied to product price, margin, and expected CVR rather than a fixed number alone.

### Correlation Is Not Causation

- Sales rising after a bid increase does not prove the bid caused the increase.
- Check seasonality, promotion, stock, product price, competitor activity, and channel traffic before assigning causality.

## 3. Beverage And Repeat-Purchase Product Framework

### Demand Structure

Separate demand into:

1. **Brand demand**
   - product and brand terms such as the main brand and zero-sugar variant.
2. **Category or function demand**
   - hydration, ion drink, exercise drink, hangover or fatigue context where policy allows, and summer refreshment.
3. **Flavor or variant demand**
   - peach, lemon, zero, powder, bottle, stick, or package-specific terms.
4. **Occasion demand**
   - exercise, outdoor activity, travel, office, hot weather, bulk purchase, or gifting.
5. **Promotion demand**
   - time deal, coupon, emergency supply event, new-product launch, or platform event.

### Product Roles

- **Defend:** branded hero products that capture existing demand.
- **Expand:** category, use-case, flavor, and new-customer products.
- **Repeat:** bundles or replenishment configurations designed for repeat purchase.
- **Test:** new flavor, new package, or seasonal promotion product.
- **Reduce:** overlapping products that split clicks without distinct price, configuration, or role.

### What The Ringti Emails Suggest

- Brand keywords were being defended while bids were gradually lowered, which is a valid efficiency approach if exposure remains sufficient.
- Generic and flavor-related contexts such as exercise drink, peach ion drink, and lemon ion drink showed additional sales signals in the eBay report.
- AI recommendation performance fluctuated materially. This should be managed as an expansion layer, not assumed to be stable simply because it previously achieved high ROAS.
- Promotion and emergency-event weeks materially affected purchase volume and ROAS, so ordinary-week and event-week baselines must be separated.
- 11st weakened while eBay improved. This is evidence of channel divergence, not enough evidence that demand transferred from one marketplace to another.

### Beverage Operating Actions

1. Protect brand demand at the lowest bid that maintains sufficient exposure.
2. Separate category, flavor, package, and occasion contexts so expansion performance can be read.
3. Use AI or recommendation campaigns for controlled expansion after excluding repeatedly weak products.
4. Prepare summer demand before peak heat rather than reacting after the peak begins.
5. Compare bundle size and AOV, not only product-level ROAS.
6. Review repeat-purchase or returning-customer data when available.
7. Keep promotion days in a separate analysis column.
8. Scale only when revenue or contribution profit grows with acceptable ROAS.

### Beverage Weekly Comment Example

> 이번 주 ROAS는 전주 대비 하락했지만, 프로모션 종료와 구매수 감소가 함께 확인되어 입찰 조정만으로 원인을 설명하기는 어렵습니다. 브랜드 수요는 현재 노출을 유지할 수 있는 범위에서 입찰가를 방어하고, 운동음료·맛·패키지 관련 확장 영역은 상품별 매출과 CVR을 기준으로 분리 검증하겠습니다. AI 추천 영역은 이전 고효율만을 기준으로 예산을 확대하지 않고, 최근 2~3주의 상품별 성과를 확인해 유지 상품과 제외 상품을 재구성하겠습니다.

## 4. Seasonal Fresh-Food Framework

### Product Lifecycle

Every seasonal product should have a lifecycle status:

| Phase | Meaning | Default Action |
|---|---|---|
| Prepare | Search and supply begin to form | Small test, listing and price readiness |
| Enter | Demand is increasing | Expand winning channel and placement |
| Peak | Demand and inventory are both strong | Concentrate budget with margin controls |
| Late | Price, quality, stock, or demand becomes unstable | Reduce broad exposure, protect profitable contexts |
| Exit | Stock ends or conversion collapses | Stop promptly and transfer budget |
| Evergreen | Stable year-round demand | Maintain by channel-product profitability |

### Required Non-Ad Inputs

Fresh-food interpretation requires:

- harvest and shipping start date;
- available inventory and expected stock-out date;
- grade, size, weight, and package;
- selling price and coupon changes;
- shipping fee and cold-chain cost;
- cancellation, damage, and refund rate;
- weather and holiday effects;
- product margin and acceptable break-even ROAS.

Without these inputs, ad data alone cannot distinguish weak advertising from weak supply, price, or product conditions.

### What The Samdamol Email Suggests

- Naver cost and purchases increased while revenue was nearly flat, causing ROAS to decline. This pattern points to weaker CVR and lower revenue per order, not merely expensive clicks.
- Shopping Search generated materially more clicks and purchases, but revenue growth did not keep pace with spend growth. Product mix and AOV need review before further scaling.
- Product performance differed sharply by product, device, placement, campaign type, and marketplace.
- Hanrabong remained efficient in several areas, but a seasonal product showing high ROAS near the end of its selling window should not automatically receive long-term budget expansion.
- Chodang corn showed increasing traffic and slight efficiency improvement, but its ROAS remained relatively low. It should be managed as an entering-season product with margin and inventory controls, not labeled a winner only because sales increased.
- Some narrow intent groups such as vacuum-packed or size-specific fish terms produced strong ROAS from small spend. These are scale candidates only after checking whether the result is repeatable.
- Kakao catalog and some ADVoost tests produced no or weak conversion. Quick test-and-stop behavior was appropriate given the number of concurrent channels.
- The account was operating too many products and media simultaneously for interpretation to remain simple. A product-channel priority matrix is necessary.

### Seasonal Fresh-Food Product-Channel Matrix

For each product, record:

| Field | Example Decision Use |
|---|---|
| Lifecycle phase | prepare, enter, peak, late, exit, evergreen |
| Inventory days | how long scaling can continue |
| Margin / break-even ROAS | whether headline ROAS is profitable |
| Best channel | Naver, 11st, Gmarket/Auction, Lotte ON, Coupang |
| Best campaign / placement | search, shopping, AI recommendation, brand, content |
| Best device / context | mobile, PC, integrated search, plus store, expanded term |
| Scale signal | repeat purchases, stable CVR, acceptable AOV |
| Stop signal | stock risk, margin loss, repeated no-conversion spend |

### Seasonal Fresh-Food Operating Actions

1. Set the product calendar before setting the media budget.
2. Allocate budget by lifecycle phase, inventory, and margin.
3. Do not keep last season's winner as the next week's default winner.
4. Move budget from exiting products to entering products before stock or demand changes become obvious.
5. Keep evergreen seafood, meat, processed goods, and seasonal fruit in separate operating tiers.
6. Diagnose `spend up, revenue flat` through CVR and AOV before changing bids.
7. Scale narrow high-ROAS terms gradually because small denominators can exaggerate efficiency.
8. Stop product ads immediately when inventory, shipping, coupon, or price conditions invalidate the campaign.
9. Compare the same product across channels before calling a marketplace weak.
10. Limit simultaneous experimental media when the product calendar already creates high volatility.

### Seasonal Fresh-Food Weekly Comment Example

> 금주 네이버는 클릭과 구매수가 증가했지만 광고비 증가 대비 매출이 정체되어 ROAS가 하락했습니다. CPC만의 문제라기보다 전환율과 주문당 매출이 함께 낮아진 구조로, 유입이 확대된 상품군의 가격·구성·판매 비중을 우선 확인해야 합니다. 초당옥수수는 시즌 진입 상품으로 노출과 구매가 증가하고 있으나 현재 수익률만으로 즉시 확대하기보다 재고, 마진, 상품 등급별 전환을 확인하며 단계적으로 예산을 늘리는 것이 적절합니다. 반면 시즌 후반 또는 재고가 불안정한 상품은 효율이 높더라도 장기 확대 대상이 아니라 잔여 판매 기간에 맞춘 단기 집중 대상으로 관리해야 합니다.

## 5. Better Weekly Reporting Format

For both categories, use:

1. **What changed**
   - exact metric movement.
2. **Why it may have changed**
   - traffic, CVR, AOV, promotion, season, stock, price, or intervention.
3. **What is confirmed versus inferred**
   - do not present hypotheses as facts.
4. **What action was taken**
   - product, bid, budget, placement, or schedule.
5. **What result will validate the action**
   - revenue growth, stable ROAS, qualified orders, repeatability, or inventory sell-through.
6. **What will happen next week**
   - maintain, scale, reduce, stop, or prepare.

## 6. Wording Corrections

Avoid:

> 비용을 줄여 ROAS가 올랐으므로 성과가 개선되었습니다.

Prefer:

> 비용 축소 폭이 매출 감소 폭보다 커 ROAS는 개선됐지만, 매출 규모도 함께 감소했습니다. 현재 결과는 성장보다 수익률 방어에 가깝고, 차주에는 고효율 상품에 제한적으로 예산을 재배분해 매출 회복 여부를 확인하겠습니다.

Avoid:

> 입찰가를 올린 결과 매출이 증가했습니다.

Prefer:

> 입찰가 상향 이후 매출이 증가했으나, 시즌 수요와 프로모션 영향도 함께 존재할 수 있습니다. 동일 상품의 노출·클릭·CVR과 비프로모션 기간 성과를 추가 비교해 입찰 조정 효과를 확인하겠습니다.

Avoid:

> ROAS 0%이므로 상품을 종료합니다.

Prefer:

> 최근 2주간 의미 있는 비용이 소진됐으나 전환이 발생하지 않았고, 상품 마진과 잔여 판매 기간을 고려할 때 추가 학습보다 예산 이동의 가치가 높아 광고를 중단합니다.
