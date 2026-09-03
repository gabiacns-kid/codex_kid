# Source-First Proposal Research Workflow

Use this reference when preparing Korean online advertising sales proposals where the user wants a NotebookLM-like source-based insight flow combined with GabiaCNS ad-operation judgment.

## Core Positioning

The workflow is not "search the web and summarize." It is:

1. infer the right research keywords from the advertiser, category, product, and ad objective;
2. collect official or high-trust sources;
3. separate verified facts, market signals, and hypotheses;
4. combine the research with existing GabiaCNS domain knowledge;
5. translate the result into media strategy, operating structure, risks, and client-facing proposal wording.

## When To Use

Use this flow when:

- the user is preparing an ad sales proposal for a new advertiser or unfamiliar category;
- the user provides a company name, URL, product category, or NotebookLM-style source summary;
- market, competitor, product, seasonality, or buyer-behavior context matters;
- the proposal needs more than generic channel recommendations;
- the advertiser is in commerce, B2B, local service, education, healthcare, finance, app, marketplace, or other category where buyer intent and product fit matter.

## Source Priority

Prefer:

- advertiser official website, store, product pages, catalog, brochure, company introduction;
- official ad platform help, notices, policies, product guides;
- public marketplace/category pages where product positioning and competitor context can be observed;
- public price-comparison, shopping, or commerce pages when relevant;
- government, industry association, credible research institutions, public filings, or established media;
- user-provided internal reports, email examples, exported ad reports, NotebookLM summaries, and uploaded files.

Avoid relying on:

- low-quality SEO blogs;
- anonymous claims with no source;
- old market reports whose date is unclear;
- unverifiable "No.1" or market-share claims;
- one marketplace screenshot as proof of the whole market.

## Research Query Inference

From the advertiser and product, generate research keywords across:

- category name: e.g. 자동차 와이퍼, 차량용품, 와이퍼 교체, 와이퍼 사이즈;
- product type: e.g. 하이브리드 와이퍼, 플랫 와이퍼, 실리콘 와이퍼, 리필 고무;
- buyer problem: e.g. 와이퍼 소음, 유막, 빗물 닦임, 장마철 와이퍼;
- competitor/brand: e.g. 보쉬 와이퍼, 불스원 와이퍼, 현대모비스 와이퍼, 킴블레이드;
- sales channel: e.g. 네이버쇼핑 와이퍼, 쿠팡 와이퍼, 다나와 와이퍼;
- ad-intent terms: e.g. 차종명 와이퍼, 사이즈 와이퍼, 자동차용품 쇼핑검색광고.

## Analysis Structure

Use this sequence:

1. Advertiser diagnosis
   - What the advertiser sells, who buys it, and what purchase barrier exists.
2. Market and search context
   - Category size, seasonality, product types, competitor positions, price bands, and buyer search behavior.
3. Product and positioning critique
   - What can be credibly claimed, what is weak, and what must not be overclaimed.
4. Media fit
   - Which channels are meaningful, not merely possible.
5. Operating strategy
   - Campaign structure, keyword/product grouping, feed/listing/landing readiness, budget concentration, and optimization logic.
6. Measurement
   - KPI hierarchy such as ROAS, CVR, AOV, qualified lead, quote, purchase, repeat purchase, LTV.
7. Client-facing proposal wording
   - Practical, defensible, and not overpromising.

## Critical Review Rules

- Treat NotebookLM or user-provided source summaries as useful starting material, not final proof.
- Re-check unstable facts such as product availability, ad product rules, pricing, market share, and platform features when they matter to the proposal.
- Label source-backed facts separately from strategic hypotheses.
- Do not inflate category research into guaranteed ad performance.
- Do not propose media expansion before checking budget, tracking, landing, product feed, creative, and sales follow-up readiness.
- For ROAS objectives, prioritize high-intent purchase surfaces before broad awareness media unless the category requires demand creation.

## Example: CAP / Automotive Wiper Proposal Logic

If the advertiser is CAP, a Korean automotive wiper manufacturer/seller, use a source-first flow like:

1. Research the online wiper market by product type:
   - conventional, flat/beam, hybrid, refill rubber;
   - synthetic rubber, silicone, graphite/graphene coating;
   - front set, rear wiper, car-model-specific size set.
2. Review competitor positions:
   - Bosch: broad recognition and value lines;
   - Bullsone: consumer brand and functional/premium coating lines;
   - Hyundai Mobis or OEM-style products: fit and trust;
   - specialty premium brands: technology/design differentiation;
   - low-cost marketplace sellers: price and compatibility breadth.
3. Identify CAP's possible position:
   - manufacturer credibility;
   - online direct price;
   - car-model fit guide;
   - refill/economy line if available;
   - premium material or coating line if supported by product facts.
4. Translate into ads:
   - Naver Shopping Search / product ads for high-intent purchase;
   - Coupang or marketplace ads when the product is listed there and ROAS tracking is available;
   - price-comparison surfaces such as Danawa/Enuri if actually available and budget permits;
   - retargeting only after site/store traffic and product events are sufficient;
   - seasonal bid and budget control around rain, monsoon, snow, holiday driving, and vehicle-inspection periods.
5. Operating principle:
   - split by car model/size intent, product type, premium vs value line, refill vs full blade, and seasonal demand;
   - optimize by ROAS, CVR, AOV, product margin, review/price competitiveness, and stock.

Client-facing example:

```text
와이퍼는 소비자가 차종과 규격을 확인한 뒤 구매하는 소모품이기 때문에, 초기 광고는 검색·쇼핑 기반의 고의도 수요를 우선 확보하는 것이 적합합니다. CAP는 제조 기반의 신뢰성과 온라인 직판 가격을 함께 설명할 수 있으므로, 단순 저가 경쟁보다는 '차종별 정확한 규격 매칭'과 '제조사가 직접 제공하는 합리적 교체 솔루션'을 전면에 두는 방향이 효과적입니다.
```

## Deliverable Template

When the user asks for a proposal using this workflow, return:

1. Research keywords inferred
2. Sources checked and reliability level
3. Market/category findings
4. Competitor and product-position map
5. Critical gaps or risks
6. Recommended positioning
7. Recommended ad products and why
8. Campaign/keyword/product grouping
9. Budget and KPI logic
10. Client-facing email or proposal text
