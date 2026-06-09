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
