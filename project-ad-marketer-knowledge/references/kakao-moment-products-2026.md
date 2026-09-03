# Kakao Moment and Kakao Ads product notes 2026

Use this reference when preparing Kakao Ads proposals, comparing Kakao with Naver, or deciding whether Kakao should be included as a core media option.

These notes are based on user-provided Kakao product guide excerpts in June 2026. Verify current Kakao Business official guides, rate cards, beta/CBT status, and account eligibility before finalizing client-facing estimates.

## Planning posture

Kakao should be considered as an alternative core media option alongside Naver, Google, and Meta.

Do not frame Kakao as only a backup. Kakao can become a main test or main campaign channel when the advertiser has:

- mobile-first inquiry or purchase flow,
- Kakao channel assets,
- marketing opt-in data,
- strong message or offer,
- event/launch/booking objective,
- need for high-reach KakaoTalk discovery,
- product catalog and pixel/SDK readiness.

Do not force Kakao when:

- there is no landing or business form,
- no consented audience exists for message ads,
- product catalog/pixel/SDK setup is missing for catalog ads,
- budget is too small for the number of Kakao products,
- the objective is pure search demand and Naver/Google have stronger intent volume.

## Performance ads

### Product Catalog

- Objective: conversion.
- Pricing: CPC.
- Role: dynamic product ad that uses linked product data to retarget and recommend products to users likely to purchase.
- Audience: optimized automatically; custom target features are not supported in product catalog ad groups.
- Purchase detargeting can be used for new-purchaser acquisition.
- Formats: catalog type and Bizboard type.
- Up to 10 linked products can be shown dynamically, but some placements may show only one product.
- Inventory: KakaoTalk, Daum, Kakao services, network inventory across mobile and PC.
- Setup dependency: catalog, pixel/SDK, representative domain, product data, product set, and in some cases profile information review for Bizboard exposure.

Critical caution:

- This is meaningful only when the advertiser has product data, a purchaseable site/app, and pixel/SDK event matching.
- Catalog item ID and pixel/SDK content_id matching matter. Keep catalog match rate high; Kakao recommends 90%+ match rate.
- Catalog menu may be available only to partnered advertisers. Verify account access before proposing as executable.

### Kakao Bizboard performance

- Role: high-reach KakaoTalk-centered display product for discovery, events, app download, traffic, lead entry, and brand interaction.
- Creative types: object, thumbnail, masking, text.
- Landing types: URL, AdView, Channel WebView, chatbot, Business Form, channel post/news, app market/store settings, Kakao service links.
- AdView can show a bridge page in the chat tab with action buttons; full view and compact view exist.
- Business Form can be connected for application, survey, event, reservation, or lead collection.
- Inventory: KakaoTalk, Daum, Kakao services, and network inventory depending on landing/material conditions.

Critical caution:

- Bizboard can be performance-oriented, but do not promise direct conversion unless the landing/offer/form is strong.
- If the advertiser lacks a website, Business Form or Channel WebView can be more realistic than URL-only landing.

### Kakao Display Ads

- Objectives: visit and conversion.
- Role: display/native ads across Kakao core services and partner inventory.
- Targeting: demographics, interests, and user actions such as cart addition, wish/product/content view, purchase, or visit where data exists.
- Creative types: image native and video native.
- Supported image ratios: 1:1, 2:1, 9:16, 4:5. Minimum 500 x 500px for 1:1 images.
- Supported video ratios: 16:9 and 9:16. Minimum 1280 x 720px for 16:9 video.
- Image catalog creative type ended on 2026-05-11. Use slide assets in image/video native creatives instead where relevant.
- Inventory: KakaoTalk, Daum, Daum Cafe, Kakao services, and partner services.

Critical caution:

- Do not treat display ads as only banner reach. They can support visit/conversion objectives, but need tracking, landing quality, and audience logic.

## Guaranteed / CPT ads

### Kakao Bizboard CPT

- Pricing: CPT, sold by time slot.
- Role: time-based high-impact exposure on KakaoTalk friend tab.
- Default unit: 10 slots per day; 2 hours per slot, 4 hours for late-night slots.
- Targeting: unavailable.
- Creative follows Bizboard base, with relaxed object/thumbnail box image guides for CPT.
- Landing types: URL, AdView, Channel WebView, chatbot, Business Form, channel post/news, web-embed channel, app market/store, Kakao service.

Use when:

- awareness, reach, launch announcement, event burst, or broad brand impact is the objective.

Avoid when:

- the campaign is judged only by CPL/CPA and budget cannot support a branding burst.

### Profile Full View

- Pricing: CPT, 24-hour exposure.
- Role: full-screen ad experience in KakaoTalk friend tab update profile flow.
- Shows profile-type material and full-view material.
- Can support image or video material.
- Can drive landing and KakaoTalk channel add.
- Device/version caveats apply; old KakaoTalk/OS versions may not support exposure.

Use when:

- campaign needs strong KakaoTalk discovery and channel-friend growth.

### Kakao Gift Home CPT

- Pricing: CPT by one-hour slots from 09:00 to 21:00.
- Landing: Kakao Gift only.
- Targeting: unavailable.
- Role: high-impact commerce exposure on Kakao Gift home.

Use when:

- advertiser sells through Kakao Gift or campaign is gift-commerce relevant.

### Focus Board PC

- Pricing: CPT by time slot.
- Role: fixed lower area in Windows KakaoTalk PC main window.
- Supports 3-10 second muted video auto-play, background/object animation, or static banner sequence.
- Metrics can be checked through Kakao Moment creative video metrics.

Use when:

- B2B, work-hour, PC-use, finance, education, enterprise, or broad PC awareness is strategically useful.

### Rich Pop All Day PC

- Pricing: CPT, 24-hour flat by weekday/weekend/holiday.
- Role: floating pop-up at Windows KakaoTalk PC login.
- Two images transition for seven seconds; users can close the ad.

Use when:

- broad PC KakaoTalk reach is needed and budget fits fixed-rate buying.

## Message ads

### Channel Message

- Audience: KakaoTalk channel friends or friend groups made from phone number/app user ID, and estimated target audiences among channel friends.
- Role: CRM-style re-engagement for owned channel audience.
- Formats: wide image, wide list, basic text, carousel, premium video.
- Pricing: CPMS.
- Smart Message can optimize recipients and creatives based on responses, but may take longer to send.
- Robot analysis report can provide demographic, interest, and demographic-by-interest charts for smart message click users.

Critical caution:

- Requires channel friend base or friend group.
- Must comply with anti-spam law and Kakao channel guidelines.
- Sending may be delayed under high-volume, smart-message, near-start-time, or recently edited group conditions.

### Personalized Message

- Audience: channel friends + owned mall/app members.
- Trigger: customer behavior event through Kakao Moment/API.
- Role: automated personalized message based on behavior, such as customer name/text/product image.
- Pricing: CPMS, message-type dependent.
- Requires API request with target information.
- Provides message performance metrics and ad response target creation.

Critical caution:

- This is not a simple media buy. It requires event data/API readiness and customer data governance.

### Brand Message

- Audience: users who agreed to receive marketing information, regardless of KakaoTalk channel friend status where eligible.
- Sender: business-verified KakaoTalk channel.
- Pricing: CPMS.
- Targeting: mainly friend group/send-target exclusion, not full Kakao Moment targeting.
- Channel-add button is available.

Critical caution:

- Confirm product availability/CBT status, consent, business-verified channel, sender profile, free opt-out phone number, and legal compliance.

### KakaoTalk Brand Pick Message

- Sender: Kakao-owned KakaoTalk Brand Pick channel.
- Audience: KakaoTalk Brand Pick channel friends selected by behavioral data.
- Role: reach new users that advertiser-owned channel messages cannot reach.
- Message must be benefit-led: coupon, points, limited free gift, immediate reward, etc.
- Reward is provided when the user clicks and stays on the advertiser page for around 10 seconds, though some landings may reward immediately.
- Also appears in Brand Pick service feed.
- Pricing: CPMS, CBT/provisional pricing may apply.
- Review required.

Critical caution:

- Treat as reward/benefit-driven discovery, not the same as owned channel CRM.
- Confirm CBT/product availability and landing/reward conditions before proposing.

## Engagement ads

### Participatory Ads

- Role: mobile-only conversion ad for lead collection.
- Requires domestic business registration number or overseas D-U-N-S on the ad account.
- Required tool: Business Form+.
- Objective: lead collection through business form style flow.
- Pixel & SDK must be selected for the campaign, but advertiser website/app script installation is not separately required for this campaign type.
- Optimization can start without rich prior data, but more recent pixel/SDK data improves optimization.

Use when:

- consultation request, event application, reservation, lead capture, survey, or simple application is the objective.

## Search ads

### Kakao Keyword Ads

- Role: CPC keyword search ads on Daum PC/mobile search premium link area, KakaoTalk #search results keyword tab, and search/content partner inventory.
- Pricing: CPC.
- Quality index considers click rate, keyword/ad relevance, and performance.
- PC Daum search can show up to 10 premium links; mobile Daum search can show up to 6.
- Content media can show text plus thumbnail-style extension material based on keyword and consumed content relevance.

Critical caution:

- Do not sell top-fixed exposure. Ranking is auction and quality-index based.
- Watch for over-spend and minus balance/day budget overrun risks when daily budget is too low or bid is too high.

### Kakao Brand Search

- Role: information content product at top of Daum search results for brand or brand-related keywords.
- Pricing: by product type, exposure area, and material format.
- Use for brand information exploration and official-content reinforcement.

### Talk Channel Search

- Role: ad in KakaoTalk search service when users search keywords.
- Formats: recommended material and custom material.
- Custom material can support CTA and external landing.
- Channel add button appears when user is not a friend.
- Pricing: CPM. Standard CPM 3,000 KRW; promotional CPM 2,000 KRW when available.
- Search service has around 10 million daily users visiting/searching in KakaoTalk search according to the provided guide excerpt.

Use when:

- KakaoTalk search discovery, channel growth, or brand search within KakaoTalk is valuable.

## Easy Ads and local map

### Easy Ads

- Simplified mobile-first Kakao ad creation platform for advertisers with owned business assets.
- Includes store promotion through KakaoTalk and Kakao Map.

### Our Store Map Ads

- Role: fixed store exposure in Kakao Map so users can discover nearby stores without searching.
- Pricing: prepaid daily fixed/CPT style.
- Term: minimum 7 days to maximum 90 days.
- Inventory: Kakao Map mobile app map view and store home.
- Up to three advertised stores can appear on one Kakao Map screen area.
- Some franchise direct-operated stores may be restricted depending on rules.

Use when:

- offline store visitation, local discovery, new opening, local coupon/promotion is the objective.

Avoid when:

- the objective is purely online lead generation without local visit relevance.

## Business Form

- Free business tool for response collection inside KakaoTalk.
- Types: quick application, survey, application/reservation.
- Can collect Kakao account-linked information such as nickname, email, and phone number after participant consent.
- Can be connected through Kakao Bizboard, business message, channel message, GiftX, Kakao Shopping Live, and other Kakao Business marketing surfaces.

Use when:

- advertiser lacks a website, needs quick applications, consultation requests, event entries, surveys, or reservations.

## Pixel & SDK

- Kakao conversion tracking tool for web/app and Kakao services.
- Supports conversion reporting, remarketing, and conversion optimization.
- Can collect non-identifiable ad cookie aid, ADID/IDFA, event type/tag, current/referrer URL, IP address, and browser user agent.
- Events that can be reported include sign-up, cart view, purchase, purchase amount, lead, service application, app install, add to cart, add to wishlist.
- Permissions: master/member structure; members can use linked pixel/SDK without full transfer.

Proposal caution:

- For serious performance campaigns, check pixel/SDK creation, ownership, member access, event setup, and ad-account linkage before launch.

## Catalog

- Catalog is a space for product data such as title, price, image, description, link, brand, category, availability, and other attributes.
- Catalog is used as ad creative input for dynamic product ads.
- Catalog menu may be provided only to partnered advertisers; verify before proposing.
- Catalog must be linked to ad account to use in Product Catalog x Conversion campaigns.
- Catalog creation requires pixel/SDK, representative domain, and catalog name.
- Product data can be linked by scheduled URL upload or manual file upload.
- Supported file formats include CSV, XLSX, XLS, TSV, XML (RSS/ATOM), up to 100MB for manual uploads.
- Google Sheets public-link scheduled upload can be used, first sheet only.
- Product list shows up to 20,000 items; user-created sets up to 50.
- Catalog item match rate compares pixel/SDK product IDs to catalog product IDs; keep 90%+ where possible.
- Bizboard exposure requires profile information and review. Profile review can take 3-5 business days.
- Banner confirm is a required process before AI-created banners can be exposed. For product names over 16 characters, Kakao AI may summarize the title; human confirmation or auto-confirm setting is needed.

Critical caution:

- AI summary in banner confirm may not perfectly match the product. Do not use auto-confirm blindly for regulated, luxury, medical, financial, or claim-sensitive products.
- Sale price effective dates are not reflected in banner confirm output, so sale_price needs periodic updates.

## 2026-07-02 Learning: Kakao Store Food Catalog Campaign For Seasonal Sales

Use this section when the user asks how to propose Kakao ads for a Kakao Store / Talk Store food advertiser that wants short-term seasonal product sales with a small budget such as KRW 1M-3M.

### 1. Newly Learned Facts

- Product Catalog ads can be positioned as the primary sales-oriented Kakao ad for Kakao Store food sellers when product linkage, catalog access, and conversion tracking are available.
- Product Catalog ads are conversion-objective, CPC-billed dynamic ads. They use linked product data and Kakao optimization to expose products to users likely to convert.
- Product Catalog ad groups are not operated like ordinary display ad groups. Audience optimization is automatic, and separate custom-target attachment is not the default operating method.
- Purchase detargeting can be used for new-purchaser acquisition, but manual segmentation such as visitor group A, cart group B, or demographic micro-groups should not be promised as a Product Catalog ad group structure.
- A Product Catalog ad can serve both as a sales campaign and as a reaction-data accumulation route. Ad click/open/conversion reactions can later support separate display, Bizboard, or message retargeting where available.
- Product sets can be selected for catalog creative operation. For seasonal fresh-food sales, this means the advertiser can focus on selected seasonal products instead of exposing every SKU, but the live product set should be kept small and coherent.
- Product sets require at least two operable products for smooth exposure. If the advertiser wants to promote only one seasonal SKU, pair it with a related set item, bundle, premium pack, or best seller.
- Catalog type should generally be used first for KRW 1M-3M seasonal sales. Bizboard type can be considered as a secondary test only after checking authority, profile review, and budget adequacy.
- If a Bizboard-type catalog exposure is available, it is usually more coherent to test Bizboard type inside the Product Catalog campaign before proposing a separate generic Bizboard visit campaign for the same sales objective.
- Kakao Click ID (`kclid`) helps connect ad-click identifiers to later conversion events under cookie-restricted environments. It is a measurement and optimization aid, not a way for the advertiser to directly identify or manage users' Kakao IDs.

### 2. Corrections To Existing Kakao Knowledge

- Do not say that Kakao Store entry alone makes conversion tracking automatic or easy. It can make product linkage more plausible, but ad account, catalog, Pixel & SDK, click ID, and service linkage still need confirmation.
- Do not say that Kakao Store advertisers can freely use Kakao ID-based retargeting. Kakao may optimize with platform signals, but the advertiser does not directly receive or operate individual Kakao IDs.
- Do not recommend many product sets as simultaneous ad groups for small budgets. Preparing multiple product sets is different from running multiple product-set ad groups at the same time.
- Do not describe Product Catalog retargeting as manual retargeting. Safer wording: automated dynamic retargeting/recommendation based on product reactions and conversion signals.
- Do not split KRW 1M-3M across Product Catalog, separate Bizboard, separate display, and messages unless there is a specific audience base and enough budget to evaluate each role.

### 3. Practical Operating Principles

For KRW 1M-3M seasonal fresh-food campaigns:

1. Start with one Product Catalog conversion campaign.
2. Use one live ad group with broad/whole audience and automatic optimization.
3. Use one live product set with 2-6 coherent seasonal SKUs.
4. Keep separate product sets as reserves, not simultaneous budget splits.
5. Use catalog type first. Add Bizboard type only if eligible and if the budget can support the test.
6. Confirm Pixel & SDK, catalog linkage, item ID/content ID matching, purchase event, and `kclid` before presenting conversion reporting as ready.
7. After the first campaign accumulates ad reactions, consider separate display/Bizboard/message retargeting only if the audience volume is meaningful.

Recommended product-set construction for seasonal food:

| Product set | Contents | Use |
|---|---|---|
| Live seasonal set A | Main seasonal SKU + bundle + premium pack + best seller | Initial campaign |
| Reserve set B | Discount or late-season stock products | Mid-season replacement |
| Reserve set C | Gift or holiday set products | Next seasonal/holiday push |

Avoid mixing unrelated food categories in one live set, such as fruit, beef, kimchi, and seafood together, unless the landing is a broad store-wide promotion. Coherent product intent improves interpretation and optimization.

### 4. Proposal And Report Wording

> 카카오스토어 입점 신선식품의 시즌 매출 활성화 목적이라면 상품 카탈로그 광고를 우선 제안드립니다. 상품 카탈로그 광고는 카카오스토어 상품을 연동해 구매 가능성이 높은 이용자에게 상품 이미지, 가격, 할인 정보 등을 자동 노출하는 전환형 광고입니다. 예산이 100만-300만 원 수준이라면 여러 광고상품으로 나누기보다 시즌 대표상품 2-6개를 하나의 상품세트로 구성해 카탈로그형 소재 중심으로 운영하는 것이 적합합니다.

> 상품 카탈로그 광고는 리타겟팅 목적의 운영이 가능하지만, 운영자가 방문자·장바구니·구매자 타겟을 세부적으로 직접 선택하는 방식은 아닙니다. 카탈로그에 연동된 상품 반응 이벤트와 전환 데이터를 기반으로 카카오가 자동으로 전환 가능성이 높은 이용자에게 상품을 추천·노출하는 구조입니다.

> 초기에는 상품 카탈로그 광고를 통해 시즌 상품 구매 전환과 상품 반응 모수 확보에 집중하고, 이후 광고 반응자 타겟이 충분히 축적되면 별도 디스플레이, 비즈보드, 메시지 캠페인을 통해 재접촉하는 단계형 운영을 권장드립니다.

> 카카오톡채널을 보유하고 있다면 상품 카탈로그 광고와 채널 메시지를 함께 활용할 수 있습니다. 카탈로그 광고는 시즌 상품에 관심을 가질 가능성이 높은 신규 이용자에게 상품을 노출하고, 채널 메시지는 기존 친구에게 쿠폰, 재입고, 마감 임박, 한정 수량 등의 메시지를 발송해 구매를 재유도하는 역할을 합니다.

### 5. Items Requiring Confirmation

- Whether the advertiser's Kakao Store / Talk Store products can be linked to a Product Catalog in the specific ad account.
- Whether the Catalog menu is available to the advertiser or requires partner/whitelist access.
- Whether Pixel & SDK is created, linked to the ad account, and collecting purchase or product-reaction events.
- Whether `kclid` is enabled and accepted through the landing/conversion route.
- Whether item IDs in catalog data match Pixel & SDK content IDs; keep match rate high.
- Whether catalog-type and Bizboard-type creative exposure are both available; Bizboard type may require profile information review and authority.
- Whether channel friend count is large enough to justify channel message budget.
- Whether fresh-food, health-food, origin, efficacy, discount, or limited-quantity claims require additional review evidence.

## 2026-07-30 update: catalog targeting and placement claims

### 1) 새로 학습한 사실

#### 제공 파일 기반 사실

- CJ Mezzomedia's August 2026 media report says a customer-file detargeting option was added to the custom-target settings of Kakao Moment Product Catalog ad groups.
- The report says Kakao Commerce catalog campaigns linked automatically to Gift and Talk Store expanded to `쇼핑탭 > 랭킹탭 > 전체`.
- The report also says performance inventory expanded to KakaoTalk's More tab game area when network placements are selected, and that some institutional finance categories became eligible in chat-list-related placements while investment advisory, investment information, asset management, and debt collection remain restricted.

#### 공식 가이드 확인 결과

- The Kakao Business Product Catalog guide accessible on 2026-07-30 still states that catalog audiences are automatically optimized and that separate custom-target functions are not supported.
- Official guide checked 2026-07-30: https://kakaobusiness.gitbook.io/main/ad/moment/performance/catalog
- Kakao's display guide states that placements can change and that the latest notices/account UI should be checked.
- Official guide checked 2026-07-30: https://kakaobusiness.gitbook.io/main/ad/moment/performance/displayad

### 2) 기존 지식에서 수정할 점

- Do not immediately present customer-file detargeting as universally available. The uploaded report and the currently accessible official catalog guide conflict.
- Do not guarantee the Ranking tab, game inventory, or financial-industry placement without checking the advertiser account, current placement guide, and industry review conditions.
- `Network placement selected` does not mean the operator can guarantee one specific game screen. Placement delivery is system-selected within the allowed inventory.

### 3) 실무 적용 원칙

1. In the live Kakao Moment account, open the Product Catalog ad-group audience settings and verify whether customer-file detargeting exists.
2. Save a screenshot/date of the UI when using a new option that is not yet reflected in the public guide.
3. Check product-catalog placement reports after launch rather than assuming the entire budget will reach the newly added shopping area.
4. For finance advertisers, confirm legal category, advertiser eligibility, creative review, and exact allowed placement before proposing the newly opened inventory.
5. Use new placement expansion as a test opportunity, not a performance guarantee.

### 4) 제안서/리포트 문장 예시

> 카카오 상품 카탈로그 광고는 커머스 지면 확장과 고객파일 제외 기능이 안내되고 있으나, 공개 가이드와 계정별 제공 화면에 차이가 있을 수 있습니다. 실제 광고계정에서 사용 가능 여부와 노출 지면을 확인한 뒤, 기존 고객 제외와 신규 고객 확장 테스트에 적용하겠습니다.

### 5) 다음 확인 필요사항

- Official Kakao notice or updated public guide confirming customer-file detargeting.
- Account eligibility and release scope for Gift/Talk Store ranking-tab catalog exposure.
- Exact game inventory, reportable placement fields, and opt-out controls.
- Detailed allowed/restricted finance subcategories and review evidence.

## 2026-08-27 변경 요약: 홈페이지 없는 소액 리드 수집 구조

### 1) 새로 학습한 사실

- 카카오톡 채널 메시지는 기존 채널 친구 또는 적법하게 구성된 친구그룹을 재접촉하는 수단이므로, 친구 모수가 없는 광고주의 신규 상담 문의 확보 수단으로 바로 사용하기에는 한계가 있다.
- 홈페이지가 없는 광고주는 카카오모먼트 광고에서 카카오 비즈니스폼을 상담 신청 경로로 연결하고, 카카오톡 채널 1:1 채팅을 보조 상담 경로로 둘 수 있다.
- 카카오 비즈니스폼은 신청·예약·설문형 응답 수집에 사용할 수 있으며, 참여자의 동의를 전제로 카카오 계정 연계 정보를 받을 수 있다.
- 공식 가이드 확인일: 2026-08-27. 확인 문서: 카카오톡 채널 메시지, 비즈니스폼 활용, 카카오톡 채널 주요 기능 안내.

### 2) 기존 지식에서 수정할 점

- `카카오톡 채널 광고`를 신규 고객 대상 메시지 발송과 동일하게 설명하지 않는다. 신규 리드 확보는 디스플레이·비즈보드 등 유입 광고와 비즈니스폼의 조합, 채널 메시지는 친구 모수 축적 후 재접촉으로 역할을 구분한다.
- 홈페이지가 없다는 이유만으로 카카오톡 채널 홈을 완전한 랜딩페이지로 간주하지 않는다. 회사·서비스·상담 절차·가격 또는 견적 기준·사례·사업자 정보가 부족하면 광고 클릭 이후 신뢰 확인 단계가 비어 있을 수 있다.
- 월 100만 원 수준에서 캠페인과 고객군을 여러 개로 나누지 않는다. 기술적으로 집행 가능한 구조와 학습·평가 가능한 구조를 구분한다.

### 3) 실무 적용 원칙

1. 월 100만 원의 홈페이지 없는 리드 광고는 하나의 상담 신청 행동에 예산을 집중한다.
2. 기본 경로는 `광고 → 비즈니스폼 제출 → 빠른 전화 상담`으로 두고, 1:1 채팅은 즉시 문의를 원하는 고객의 보조 경로로 운영한다.
3. 비즈니스폼에는 이름·연락처 외에 지역, 관심 서비스, 이용 시기, 상담 가능 시간, 예산·자격 등 업종별 선별 질문을 포함한다.
4. KPI는 양식 제출수와 제출당 비용만 보지 않고 정상 연락 가능 문의, 상담 연결, 견적·방문, 계약까지 단계별로 관리한다.
5. 광고 시작 전 채널 홈에 회사 소개, 서비스 범위, 상담 절차, 가격 또는 견적 기준, 사례·후기, 자주 묻는 질문, 사업자 정보, 상담 시간, 개인정보 안내를 준비한다.
6. 친구와 마케팅 수신 동의 모수가 충분히 쌓인 뒤 채널 메시지 또는 조건이 충족되는 메시지 광고를 2단계 재접촉 수단으로 검토한다.

### 4) 제안서/리포트 문장 예시

> 별도 홈페이지가 없어도 카카오 안에서 상담 신청을 받을 수 있습니다. 초기에는 채널 친구 수 확대보다 광고에서 비즈니스폼으로 바로 연결해 실제 상담 가능한 문의를 확보하고, 채널 메시지는 친구 모수가 쌓인 이후 재상담과 프로모션 안내에 활용하는 구조를 권장드립니다.

> 월 100만 원은 여러 캠페인으로 나누기보다 하나의 상담 신청 캠페인에 집중합니다. 성과는 신청서 제출 건수보다 정상 연락 가능 문의와 실제 상담 연결률을 기준으로 평가하겠습니다.

### 5) 다음 확인 필요사항

- 광고계정에서 사용할 수 있는 비즈니스폼 연결 광고 유형과 심사 조건
- 업종별 개인정보·광고심의·필수 고지 항목
- 채널 친구 수, 마케팅 수신 동의 데이터, 기존 상담 DB 규모
- 문의 접수 후 첫 연락 시간과 상담 결과를 광고 데이터에 돌려줄 수 있는 관리 체계
