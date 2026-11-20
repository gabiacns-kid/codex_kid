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

## 2026-09-04 추가 확인: 자사몰 행동 기반 카카오 메시지 구현 범위

### 1) 새로 학습한 사실

- 카카오톡 채널의 `웰컴 메시지`는 사용자가 채널을 친구로 추가한 직후 자동 발송되는 채널 관리자센터 기본 기능이다. 자사몰 회원가입 완료를 조건으로 발송되는 메시지가 아니며, 별도 CRM/API 연동 없이 설정할 수 있다.
- 주문 확인·결제 완료·배송 안내는 알림톡의 대표적인 정보성 메시지 영역이다. 다만 카카오모먼트 광고 설정이 아니라 카카오 비즈메시지 API와 공식 딜러사, 또는 쇼핑몰 솔루션에 이미 연결된 알림톡 기능을 통해 구현한다.
- 기존 카카오톡 채널 친구에게 프로모션·신제품·재입고·쿠폰을 일괄 발송하는 것은 카카오모먼트 채널 메시지에서 직접 운영할 수 있다.
- 회원가입 완료, 상품 조회, 장바구니 이탈 등의 고객 행동을 조건으로 즉시 발송하는 개인화 메시지는 카카오모먼트 소재 등록만으로 구현되지 않는다. 자사몰 이벤트 수집, 수신자 식별자, 광고성 정보 수신 동의, 카카오모먼트 API 권한·화이트리스트, 발송 요청 개발이 필요하다.
- 개인화 메시지는 발송 채널의 친구에게만 발송된다. 전화번호 또는 앱유저아이디가 채널 친구로 확인되지 않으면 발송 요청이 취소된다.
- 브랜드 메시지는 적법한 광고성 정보 수신 동의자를 대상으로 채널 친구가 아닌 사용자에게도 발송할 수 있으나, 단순 일괄 DB 업로드 발송과 실시간 행동 트리거 자동화는 구분해야 한다. 실시간 자동화에는 CRM/마케팅 자동화와 API 연동이 추가로 필요하다.
- 식별되지 않은 단순 방문자나 이탈자에게 메시지를 임의로 발송할 수 없다. 익명 방문자 재접촉은 픽셀 기반 디스플레이 리타겟팅 영역이며 메시지 광고만 제안하는 경우 범위에서 제외한다.

### 2) 기존 지식에서 수정할 점

- `주문·배송 안내는 가능`이라고만 쓰지 말고 `알림톡 연동이 이미 구축돼 있으면 운영 가능, 미구축이면 비즈메시지 API·공식 딜러사 연동 필요`로 작성한다.
- `웰컴 메시지`와 `회원가입 완료 메시지`를 같은 기능처럼 설명하지 않는다. 전자는 채널 친구 추가 이벤트, 후자는 자사몰 회원 이벤트다.
- `장바구니 이탈 쿠폰은 조건부 가능`이라는 표현에는 채널 친구 여부, 회원 식별, 마케팅 동의, 이벤트·API 연동 조건을 함께 적는다.
- 카카오모먼트 화면에서 메시지 소재를 만드는 행위와 자사몰 행동 데이터를 이용해 발송 요청을 자동화하는 개발 영역을 분리한다.

### 3) 실무 적용 원칙

카카오 메시지 제안은 다음 세 단계로 나눈다.

1. 기본 운영: 채널 친구 추가 웰컴 메시지, 기존 친구 대상 채널 메시지.
2. 외부 서비스 연동: 주문·결제·배송 알림톡. 기존 쇼핑몰 솔루션 연동 여부를 먼저 확인하고 없으면 공식 딜러사/API 구축 범위를 산정한다.
3. CRM 자동화: 회원가입, 상품 조회, 장바구니 이탈, 재입고 관심 등의 행동 기반 메시지. 이벤트·식별·동의·친구 여부·API 권한·발송 로직을 설계한 뒤 구축한다.

행동 기반 메시지는 `가능한 광고 기능`으로만 소개하지 말고 초기 구축과 지속 운영이 필요한 CRM 프로젝트로 분류한다.

### 4) 제안서 문장 예시

> 카카오톡 채널 친구에게 발송하는 프로모션 메시지와 채널 추가 직후의 웰컴 메시지는 별도 개발 없이 운영할 수 있습니다. 주문·배송 안내는 자사몰에 알림톡 연동이 이미 구축되어 있는지 먼저 확인해야 하며, 미구축 상태라면 공식 딜러사 또는 비즈메시지 API 연결이 필요합니다. 회원가입 완료, 상품 조회, 장바구니 이탈을 조건으로 한 자동 메시지는 단순 광고 설정 범위를 넘어 자사몰 이벤트·회원 식별·수신 동의·API 또는 CRM 연동이 필요한 2단계 고도화 과제로 제안합니다.

### 5) 다음 확인 필요사항

- 조지루시 자사몰의 쇼핑몰 솔루션과 현재 알림톡 사용 여부
- 카카오톡 채널 친구 수와 광고성 정보 수신 동의 DB 규모
- 회원 전화번호·앱유저아이디와 자사몰 행동 이벤트의 연결 가능 여부
- 카카오모먼트 개인화 메시지 API 권한 및 광고계정 화이트리스트 보유 여부
- CRM 또는 마케팅 자동화 솔루션 사용 여부와 내부 개발 리소스

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

## 2026-09-04 변경 요약: 브랜드 메시지의 자사 고객 DB와 카카오 타겟 구분

### 1) 새로 학습한 사실

- 카카오모먼트 브랜드 메시지는 광고주가 적법하게 확보한 광고성 정보 수신 동의 고객의 전화번호 또는 앱유저아이디를 업로드해 `브랜드 타겟`을 생성하는 구조다.
- 발송 대상에서 `브랜드 타겟 - 채널 친구`를 선택하면 브랜드 타겟 가운데 해당 카카오톡 채널의 친구를 제외하고 비친구에게만 발송할 수 있다.
- 비친구에게 채널추가 버튼이 포함된 메시지를 보내고, 이미 친구인 이용자에게는 채널추가 버튼을 제외하는 구성도 지원한다.
- 이는 카카오가 보유한 관심사·행동 데이터로 불특정 잠재고객을 선별하는 오픈 타게팅 상품이 아니다. 광고주의 동의 고객 DB와 카카오톡 메시지 수신 가능 이용자를 카카오가 매칭하는 방식이다.
- 카카오 행동 데이터로 선별한 신규 이용자에게 카카오 소유 채널을 통해 보내는 `카카오톡 브랜드픽 메시지`와 광고주 동의 고객 DB를 이용하는 `브랜드 메시지`를 구분한다.
- 공식 가이드 확인일: 2026-09-04. 브랜드 메시지는 현재 일부 광고계정 대상 CBT로 안내되어 있어 실제 계정 제공 여부를 확인해야 한다.

### 2) 기존 지식에서 수정할 점

- `자사몰 광고 수신 동의 고객이면 모두 브랜드 메시지 발송 가능`이라고 단정하지 않는다. 광고성 정보 수신 동의 화면과 개인정보의 마케팅 목적 이용 및 카카오 채널 메시지 발송에 대한 적법한 근거가 필요하다.
- 이메일 또는 문자 수신에만 동의한 고객을 카카오톡 메시지 대상으로 그대로 사용할 수 있다고 설명하지 않는다. 실제 동의 문구와 개인정보 처리방침을 확인한다.
- `카카오 내 고객 타겟`이라는 표현을 쓸 때 플랫폼 관심사 타겟과 광고주 고객 DB 매칭을 혼용하지 않는다.

### 3) 실무 적용 원칙

1. 자사몰 회원 중 광고성 정보 수신 동의 고객을 추출하고, 동의 일시·경로·문구·철회 상태를 확인한다.
2. 카카오가 요구하는 동의 화면 증빙을 등록한 뒤 전화번호 또는 앱유저아이디 파일로 브랜드 타겟을 만든다.
3. 채널 신규 친구 확보가 목적이면 발송 범위를 `브랜드 타겟 - 채널 친구`로 설정하고 채널추가 버튼을 사용한다.
4. 발송 가능한 모수는 업로드 수와 같지 않다. 카카오톡 메시지 수신 가능 여부, 식별자 매칭, 동의·차단 상태 등에 따라 줄어들 수 있으므로 실제 예상 모수를 계정에서 확인한다.
5. 비즈니스 인증 채널, 무료 수신거부 전화번호, 개인정보 위탁·처리 고지, CBT 제공 여부를 집행 전에 점검한다.

### 4) 제안서/리포트 문장 예시

> 브랜드 메시지는 카카오의 불특정 이용자를 대상으로 보내는 광고가 아니라, 자사몰에서 적법하게 광고성 정보 수신에 동의한 고객 DB를 카카오톡 이용자와 매칭해 발송하는 상품입니다. 이 가운데 기존 채널 친구를 제외하면 비친구 고객에게만 채널추가 버튼이 포함된 메시지를 보내 신규 친구 확보에 활용할 수 있습니다.

### 5) 다음 확인 필요사항

- 해당 광고계정의 브랜드 메시지 CBT 이용 권한
- 자사몰 수신 동의 문구가 카카오 채널 메시지 발송과 마케팅 목적 이용을 포괄하는지 여부
- 업로드 가능한 전화번호 또는 앱유저아이디의 품질과 철회 고객 제외 여부
- 비즈니스 인증 채널과 무료 수신거부 전화번호 등록 상태

공식 확인 경로: https://kakaobusiness.gitbook.io/main/ad/moment/messagead/brandmessage/new

## 2026-09-04 추가 확인: 관심사 타겟 기반 비친구 메시지 발송 범위

### 1) 새로 학습한 사실

- 채널 메시지의 데모그래픽·지역·관심사·업종·광고반응 타겟 설정은 원칙적으로 해당 카카오톡 채널의 `기존 친구 중` 발송 대상을 좁히거나 우선순위를 정하는 기능이다.
- 채널 메시지의 `새로 추가되는 친구에게도 메시지 발송` 옵션은 비친구를 찾아 친구로 전환하는 광고가 아니다. 발송 시작일부터 종료일까지 다른 경로를 통해 새로 친구가 된 이용자에게 동일 메시지를 후속 발송하는 기능이다.
- 광고주의 동의 고객 DB가 없는 상태에서 불특정 카카오 이용자를 관심사로 골라 광고주 채널 명의의 메시지를 먼저 보내고 친구 추가를 유도하는 일반 메시지 상품은 공식 가이드상 확인되지 않는다.
- 카카오 행동 데이터 기반 신규 도달이 가능한 브랜드픽 메시지는 카카오 소유 브랜드픽 채널 친구를 대상으로 하는 별도 상품이다. 광고주 채널 명의의 일반 메시지나 직접적인 채널 친구 추가 광고와 동일하게 설명하지 않는다.

### 2) 기존 지식에서 수정할 점

- `채널 메시지에서 관심사 타겟을 설정할 수 있다`는 설명에는 반드시 `채널 친구 모수 안에서`라는 범위를 붙인다.
- `새 친구에게도 보내기`를 신규 친구 획득 기능으로 표현하지 않는다.
- 메시지형 신규 도달이 필요하다는 이유만으로 브랜드픽을 채널 친구 확보 상품으로 단정하지 않는다. 발송 주체, 수신 대상, 혜택·리워드, 랜딩과 실제 채널추가 경로를 별도로 확인한다.

### 3) 실무 적용 원칙

1. 고객 DB가 없고 채널 친구도 적다면 메시지 광고만으로 신규 친구를 모집한다는 제안은 하지 않는다.
2. 신규 친구 확보는 비즈보드·디스플레이·톡채널 검색 등 비메시지 광고에서 채널추가 경로를 연결하고, 친구가 된 뒤 채널 메시지로 후속 관리한다.
3. 메시지 광고만 검토해야 한다면 `기존 친구 세분 발송`, `적법한 동의 DB 기반 브랜드 메시지`, `브랜드픽 신규 도달` 중 어떤 구조인지 명확히 구분한다.

### 4) 제안서/리포트 문장 예시

> 채널 메시지의 관심사 타게팅은 기존 채널 친구 안에서 발송 대상을 선별하는 기능입니다. 고객 동의 DB가 없는 상태에서 불특정 관심사 이용자에게 광고주 채널 명의의 메시지를 먼저 보내 친구 추가를 유도하는 방식은 일반 채널 메시지나 브랜드 메시지로 운영하기 어렵습니다.

### 5) 다음 확인 필요사항

- 브랜드픽 메시지의 현재 CBT 제공 범위, 채널추가 버튼 및 랜딩 지원 범위
- 광고계정별 메시지 만들기 메뉴와 신규 기능 제공 여부
- 비메시지 광고에서 채널추가를 최적화 목표 또는 랜딩으로 사용할 수 있는 최신 상품 범위

공식 확인 경로:

- 채널 메시지 발송 대상: https://kakaobusiness.gitbook.io/main/ad/moment/messagead/channelmessage/new/send
- 브랜드 메시지: https://kakaobusiness.gitbook.io/main/ad/moment/messagead/brandmessage

## 2026-09-04 추가 확인: 브랜드 타겟의 친구·비친구 판별 시점

### 1) 새로 학습한 사실

- 자사몰 CRM 단계에서는 전화번호 고객이 광고주의 카카오톡 채널 친구인지 직접 확인하기 어렵다.
- 카카오모먼트에서 광고 수신 동의 고객의 전화번호 또는 앱유저아이디를 브랜드 타겟으로 업로드하면, 먼저 카카오톡 채널 메시지 발송이 가능한 전체 매칭 모수가 제공된다.
- 이후 브랜드 메시지 발송 대상 설정에서 `브랜드 타겟`, `브랜드 타겟 + 채널 친구`, `브랜드 타겟 - 채널 친구` 중 범위를 선택하면 카카오가 내부적으로 친구 여부를 구분하여 발송한다.
- 채널추가 버튼을 적용하면 실제 발송 시점에 비친구에게는 채널추가 버튼이 포함되고, 친구에게는 해당 버튼이 제외된 버전이 발송된다.
- 발송 후에는 메시지 보고서에서 채널 친구 여부에 따른 성과를 집계 단위로 확인할 수 있다.
- 공식 공개 가이드에서는 광고주에게 고객별 친구·비친구 여부가 표시된 명단을 내려주는 기능을 확인할 수 없다. 개인정보 보호 관점에서 개인 단위 CRM 속성으로 회수할 수 있다고 제안하지 않는다.

### 2) 기존 지식에서 수정할 점

- 브랜드 타겟 등록과 동시에 고객별 친구 여부를 CRM에 표시할 수 있다고 설명하지 않는다.
- 메시지 미리보기의 `친구 버전 보기`는 친구·비친구별 소재 형태를 확인하는 기능이지 개별 고객의 친구 상태 조회 기능이 아니다.
- 친구 상태는 변할 수 있으므로 업로드 시점의 예상 모수와 실제 발송 시점의 친구·비친구 발송 건수가 완전히 같다고 보장하지 않는다.

### 3) 실무 적용 원칙

1. 업로드 전에는 친구 여부를 추정하지 않고 적법한 동의 고객만 정제한다.
2. 업로드 후 전체 메시지 발송 가능 매칭 모수를 확인한다.
3. 신규 친구 전환 목적이면 `브랜드 타겟 - 채널 친구`를 선택하여 비친구 집계 모수와 예상 비용을 확인한다.
4. 실제 성과는 발송 후 친구 여부별 발송·열람·클릭·채널추가 지표로 확인한다.
5. 고객별 친구 상태 명단을 자사 CRM으로 되가져오는 구조는 공식 제공 여부가 확인되기 전까지 제안하지 않는다.

### 4) 제안서/리포트 문장 예시

> 자사몰 고객의 카카오톡 채널 친구 여부를 CRM에서 사전에 확인하는 방식은 아닙니다. 동의 고객 DB를 브랜드 타겟으로 등록한 뒤 카카오모먼트 발송 설정에서 기존 친구를 제외하고, 발송 후 보고서에서 친구 여부별 성과를 집계해 확인합니다.

### 5) 다음 확인 필요사항

- 실제 CBT 계정의 발송 설정 화면에서 범위별 예상 모수와 예상 비용이 어떻게 표시되는지
- 브랜드 메시지 보고서에서 제공되는 친구·비친구별 세부 지표와 다운로드 항목
- API형 브랜드 메시지에서 공식 딜러사가 제공하는 친구 상태 관련 집계 범위

공식 확인 경로: https://kakaobusiness.gitbook.io/main/ad/moment/messagead/brandmessage/new

## 2026-09-04 추가 확인: 브랜드 메시지 단가와 제공 경로

### 1) 새로 학습한 사실

- 카카오모먼트에서 직접 생성하는 브랜드 메시지는 공식 가이드상 일부 광고계정 대상 CBT로 안내된다.
- 카카오모먼트 CBT 표시 단가는 채널 친구 20원/건, 채널 비친구 정가 40원/건이며 비친구는 현재 30원/건의 CBT 프로모션가가 표시되어 있다.
- 카카오모먼트 메시지 과금은 CPMS이며, 카카오모먼트 공통 구매 가이드상 입력 단가는 VAT 미포함이고 실제 결제에는 VAT 10%가 포함된다.
- 별도로 브랜드 메시지 API 상품이 공식 딜러사 경로로 안내되고 있다. 공식 페이지에는 공통 단가가 공개되지 않았으며 딜러사별 서비스 범위, 계약 조건, API·솔루션 이용료와 최소 물량을 확인해야 한다.
- 브랜드 메시지는 CRM의 고객 DB를 생성·관리하는 완전한 CRM 솔루션이라기보다, 광고주가 보유한 동의 고객 DB를 카카오톡에서 활성화하는 메시지 발송·성과 측정 채널로 보는 것이 정확하다.

### 2) 기존 지식에서 수정할 점

- `브랜드 메시지는 전부 CBT` 또는 `누구나 카카오모먼트에서 직접 집행 가능`이라고 단정하지 않는다. 카카오모먼트 CBT형과 공식 딜러사 API형을 구분한다.
- CBT 프로모션가 30원을 영구 단가로 제안하지 않는다. 견적 시점의 계정 화면과 프로모션 종료 여부를 확인한다.
- 공식 딜러사 API형에 카카오모먼트 CBT 단가를 그대로 적용하지 않는다.

### 3) 실무 적용 원칙

1. 먼저 광고계정에 브랜드 메시지 메뉴와 CBT 권한이 있는지 확인한다.
2. 직접 집행이 불가능하면 공식 딜러사 API형의 연동비·월 기본료·건당 단가·최소 물량·계약기간을 비교한다.
3. 예산은 `실제 발송 성공 건수 × 적용 단가 + VAT + 대행/딜러 비용`으로 구분한다.
4. 비친구 신규 전환 목적이면 `브랜드 타겟 - 채널 친구` 모수를 기준으로 예상 발송비와 채널추가당 비용을 산정한다.

### 4) 제안서/리포트 문장 예시

> 카카오모먼트 직접 집행형 브랜드 메시지는 현재 일부 광고계정에 한해 CBT로 제공되며, 비친구 발송 단가는 공식 가이드상 건당 30원의 프로모션가가 적용되고 있습니다. 실제 이용 권한과 단가는 집행 시점에 확인하며, 직접 집행 권한이 없을 경우 공식 딜러사를 통한 API형 운영 조건을 별도로 비교합니다.

### 5) 다음 확인 필요사항

- 해당 광고계정의 카카오모먼트 브랜드 메시지 CBT 권한
- 비친구 30원 프로모션의 종료일과 정가 전환 시점
- 공식 딜러사 API형의 건당 단가, 구축비, 월 기본료, 최소 물량, 계약기간
- 브랜드 메시지와 자사 CRM 간 자동 동기화 및 수신철회 반영 방식

공식 확인 경로:

- 카카오모먼트 브랜드 메시지: https://kakaobusiness.gitbook.io/main/ad/moment/messagead/brandmessage
- 카카오모먼트 브랜드 메시지 만들기: https://kakaobusiness.gitbook.io/main/ad/moment/messagead/brandmessage/new
- 브랜드 메시지 API 및 공식 딜러사: https://kakaobusiness.gitbook.io/main/ad/brandmessage

## 2026-11-17 변경 요약: 비즈보드 리타겟팅 설계와 대행사·개발사 역할 구분

### 1) 새로 학습한 사실

- 카카오 픽셀·SDK가 정상 설치되어 있으면 카카오 광고 클릭자뿐 아니라 검색광고·직접 유입 등 다른 경로로 사이트를 방문한 이용자도 식별 가능한 범위에서 카카오모먼트 맞춤타겟의 재접촉 모수로 활용할 수 있다.
- 기본 페이지 방문은 `PageView`, 상품·서비스 상세 조회는 `ViewContent`, 상담·참여 완료는 `Participation` 또는 `Consulting` 등 목적에 맞는 이벤트로 구분할 수 있다. 문의 페이지 방문 후 미완료자는 `문의 페이지 진입 모수 포함 + 상담 완료 이벤트 모수 제외` 조합으로 구성한다.
- 상품 ID나 서비스 태그는 이벤트에 부가 정보를 함께 전달할 수 있을 때 세부 상품군별 오디언스 구분에 활용할 수 있다. 다만 모수가 작으면 지나친 세분화가 집행 가능 규모를 약화시킬 수 있다.
- GTM은 카카오 픽셀 설치의 필수 조건이 아니다. 홈페이지 개발·유지보수 업체가 소스에 직접 픽셀과 이벤트 코드를 삽입하는 방식도 가능하다.
- 카카오 공식 가이드의 픽셀·SDK 이벤트 예상 모수는 최근 180일 범위로 안내된다. 반면 광고반응타겟 등 다른 오디언스의 보유 기간과 동일한 개념으로 혼용하지 않는다.

### 2) 기존 지식에서 수정할 점

- 모든 비즈보드 캠페인에 픽셀이 반드시 필요하다고 설명하지 않는다. 도달·사이트 방문 목적 캠페인은 픽셀 없이도 집행할 수 있지만, 방문자 리타겟팅과 사이트 내 전환 측정·최적화에는 픽셀 및 이벤트 수집이 필요하다.
- 광고대행사가 홈페이지 코드 설치와 오류 수정을 기본 업무로 수행한다고 약속하지 않는다. 대행사는 측정 항목과 이벤트 명세를 제안하고 광고계정 연동·수집 확인·오디언스 및 캠페인 설정을 담당하며, 실제 소스 삽입과 개발 오류 수정은 광고주 또는 홈페이지 유지보수 업체의 업무로 구분한다.
- `픽셀만 설치하면 문의 미완료자를 자동 식별한다`고 단정하지 않는다. 문의 페이지 진입과 완료가 서로 다른 이벤트로 정상 수집되어야 제외 조합을 만들 수 있다.

### 3) 실무 적용 원칙

1. 1단계는 전 페이지 `PageView`로 전체 방문자 모수를 확보한다.
2. 2단계는 핵심 상세페이지 `ViewContent`와 상담 완료 이벤트를 추가하여 상세 관심자와 문의 미완료자를 구분한다.
3. 상품 ID·태그·구매금액 등 고도화 데이터는 실제 예산과 오디언스 규모가 세분 운영을 지탱할 때만 개발 범위에 포함한다.
4. 광고대행사는 이벤트 정의서, 픽셀-광고계정 연동, 수집 상태 검수, 맞춤타겟 생성 및 리타겟팅 캠페인 운영을 맡고, 광고주·개발사는 코드 설치, 동의·개인정보 고지, 완료 신호 구현과 오류 수정을 맡는다.
5. 개발 협조가 어렵다면 카카오 비즈니스폼·챗봇처럼 카카오 내부에서 완료 신호를 확인할 수 있는 경로를 우선 검토한다.

### 4) 제안서/리포트 문장 예시

> 초기에는 전체 방문자를 수집할 수 있는 기본 픽셀 설치부터 시작하고, 이후 상품 상세 조회와 상담 완료 이벤트를 추가해 관심 방문자와 문의 미완료자를 구분하겠습니다. 가비아CNS는 측정 항목 정의, 광고계정 연동, 수집 확인과 리타겟팅 운영을 담당하며, 홈페이지 코드 삽입과 개발 오류 수정은 광고주의 유지보수 업체와 협업하여 진행합니다.

### 5) 다음 확인 필요사항

- 랜딩페이지의 완료 URL 또는 AJAX·팝업 방식 등 실제 문의 완료 신호 구현 구조
- 홈페이지 유지보수 업체의 직접 설치 또는 GTM 설치 지원 가능 여부와 작업 범위
- 카카오 픽셀·SDK 계정 권한, 광고계정 연동 상태, 이벤트별 실제 예상 모수
- 개인정보 처리방침·쿠키 동의 고지와 맞춤형 광고 활용에 필요한 내부 검토
- 비즈보드 랜딩 유형과 픽셀·SDK 메뉴·이벤트 명칭의 집행 시점 최신 화면

공식 확인 경로(확인일: 2026-11-17):

- 카카오 비즈보드: https://kakaobusiness.gitbook.io/main/ad/moment/performance/talkboard
- 카카오 픽셀·SDK: https://kakaobusiness.gitbook.io/main/tool/pixel-sdk
- 픽셀·SDK 설치: https://kakaobusiness.gitbook.io/main/tool/pixel-sdk/install
- 픽셀·SDK 연동: https://kakaobusiness.gitbook.io/main/tool/pixel-sdk/linkage

## 2026-11-19 변경 요약: 인스타툰 파생 소재와 서울 한정 전용관 트래픽 운영

### 1) 새로 학습한 사실

- 카카오 비즈보드는 짧은 문구와 오브젝트·썸네일 중심의 압축형 소재이므로 여러 장을 순서대로 소비하는 인스타툰 원본을 그대로 전달하기 어렵다.
- 전용관 유입이 주 목표라면 비즈보드 방문 캠페인만으로도 집행 가능하지만, 사업 취지와 사례를 더 설명해야 하면 디스플레이 광고를 함께 운영해 역할을 나누는 편이 적합하다.
- 카카오의 데모그래픽 지역은 사용자의 거주지역을 추정한 값이며 시·도 단위 설정이 가능하다. 따라서 서울특별시 한정은 설정할 수 있지만 서울 소재 기업의 재직 여부까지 보장하지 않는다.
- 카카오 픽셀의 `PageView`는 전용관 방문 측정에 사용할 수 있고, 상세 콘텐츠 소비를 분리하려면 `ViewContent`나 별도 태그·커스텀 이벤트가 추가되어야 한다.

### 2) 기존 지식에서 수정할 점

- 인스타툰을 비즈보드에 단순 축소해 사용한다고 제안하지 않는다. 핵심 장면·헤드라인·CTA를 압축한 비즈보드 소재와 설명력이 높은 디스플레이 소재를 별도로 제작한다.
- 서울 지역 설정을 서울 소재 기업 타겟팅과 동일시하지 않는다. 서울 지역 설정을 고정한 뒤 관련 관심군과 소재 내 자격 문구를 함께 사용한다.
- 전용관 `PageView`를 콘텐츠 상세 조회나 영상 소비와 동일하게 보고하지 않는다.

### 3) 실무 적용 원칙

1. 비즈보드는 전용관 방문 확대, 디스플레이는 사업 메시지·사례 전달 역할로 구분한다.
2. 지역은 서울특별시로 고정하고 수도권·전국 확장은 제외한다. 확장 테스트가 필요하면 서울 내 관심군 범위만 조정한다.
3. 소재에는 `서울 소재 기업 대상`을 명시해 이용자가 참여 자격을 스스로 판단하게 한다.
4. 성과 비교는 비즈보드와 디스플레이의 CTR만이 아니라 랜딩페이지 조회수와 조회당 비용을 우선한다.
5. 픽셀 설치가 불가능하면 UTM과 사이트 분석도구로 매체·캠페인·소재별 유입을 구분하되, 카카오 내부의 상세 행동 최적화·리타겟팅 한계는 별도로 고지한다.

### 4) 제안서/리포트 문장 예시

> 카카오 비즈보드는 짧은 메시지로 전용관 방문을 확대하고, 디스플레이 광고는 사업 취지와 참여 사례를 보다 충분히 전달하는 역할로 구분합니다. 두 광고 유형 모두 서울특별시를 필수 지역으로 설정하며, 소재에도 서울 소재 기업 대상임을 명시합니다.

### 5) 다음 확인 필요사항

- 광고계정에서 서울특별시 지역과 관련 관심·업종 타겟을 조합했을 때의 실제 예상 모수
- 비즈보드·디스플레이별 제작 규격과 파생 소재 수량
- 전용관 `PageView`, 상세 콘텐츠 조회, 영상 재생, 신청 링크 이동의 이벤트 설치 가능 여부
- 카카오 픽셀·SDK 권한 및 잡코리아 내부 개발·유지보수팀의 설치 지원 범위

공식 확인 경로(확인일: 2026-11-19):

- 카카오모먼트 기본 안내: https://kakaobusiness.gitbook.io/main/ad/moment/intro
- 카카오 비즈보드: https://kakaobusiness.gitbook.io/main/ad/moment/performance/talkboard
- 카카오 성과형 광고: https://kakaobusiness.gitbook.io/main/ad/moment/performance
- 카카오 픽셀·SDK 설치: https://kakaobusiness.gitbook.io/main/tool/pixel-sdk/install
