# Kakao Moment ASAP and Operations Playbook 2026

Use this reference when the user asks about Kakao Moment sales strategy, Gift x Moment packages, Kakao ad/service structure, catalog updates, campaign optimization, event friend messages, ad-response targeting, budget scenarios, conversion optimization, Pixel & SDK readiness, or ASAP partner programs.

This file is based on user-provided partner/internal guide text dated around 2026. Treat package amounts, CBT/beta availability, support programs, free cash, and booking details as partner-guide information that must be rechecked with Kakao before client-facing use.

## Core Strategic Position

Kakao should not be positioned only as "another DA channel." Naver GFA, Meta, and Google can also create discovery and retargeting. The stronger Kakao position is:

> Kakao is a relationship-conversion media layer: it can connect discovery in KakaoTalk/Kakao services with Kakao channel, Business Form, Kakao Sync, Pixel & SDK, ad-response targeting, and message re-contact when permissions and data are properly set.

Do not imply that an ad click alone creates message permission. The safe commerce funnel is:

> Product catalog ad -> product detail / advertiser mall visit -> Kakao Sync signup or channel-friend conversion -> consented user / channel friend -> channel message, personalized message, event friend message, or eligible brand message re-contact.

## Moment x Gift Package

2026 "Moment x Gift package" means: when the advertiser spends the package amount as Kakao Moment ad cost, Kakao Gift ad products/services are supported according to the package.

Package guide period: 2026-01-01 to 2026-12-31.

| Package | Budget excluding VAT | Talk channel send date check | Spend period | Required rule |
|---|---:|---|---|---|
| Ad tab LNB 3rd / season tab | KRW 400M | Required | 30 days including Gift exposure date | Only Gift landing ads count |
| Splash/live package | KRW 250M | Required | 30 days including Gift exposure date | Only Gift landing ads count |
| Ad tab LNB 6th | KRW 100M | Not required | 14 days including Gift exposure date | Only Gift landing ads count |
| Talk channel package | KRW 50M | Required | 14 days including Gift exposure date | Only Gift landing ads count |

### 2026 Changes vs 2025

- 2025: some large packages required guaranteed ads.
- 2026: guaranteed and performance ads can both count.
- Still recommend spending 50% or 30%+ around key Gift exposure dates depending on package/schedule.
- Exposure period can be negotiated within 10% of contract period; no carryover, only within the same month.
- If Gift booking issues require period changes, discuss with Kakao and follow internal guide.

### Package Execution Rules

- Spend must reach at least the package amount within the required period. Even a small shortfall violates the guide.
- Only ads in the whitelisted package Moment account with Gift landing count.
- Package amount can include Moment DA, Bizboard, and message costs. Profile Full View and Focus Board also count if executed through Moment.
- Messages sent from Channel Admin Center do not count.
- A dedicated Moment account and whitelisting are required.
- Do not create campaigns before whitelisting. If campaigns are created before whitelisting, deleting them may not resolve system limitations.
- Campaign URLs must be base URLs without existing `input_channel_id=####`. The package account automatically attaches a dedicated inflow channel ID after whitelisting.
- Kakao Shopping Live landing does not count.
- For LNB 6th, first-screen exposure may not be guaranteed depending on Gift service order; priority follows confirmed execution.

### Free Cash Notes

- A free-cash support amount equal to 10% of package price may be provided for convenience and Kakao ad x Gift synergy.
- If a Gift season package includes major Gift season inventory such as season tab, splash, or talk channel message, free cash is not provided.
- Free cash is paid to the Gift package account and can be used only for Gift landing.
- It must be spent within the agreed Moment package operation period; unused amount expires.
- Free cash is manually issued around 90% paid spend. Request 2-3 business days before the expected 90% point.
- Free cash cannot be prepaid.
- After activation, free cash spends before paid cash across all campaigns. It cannot be paused, recalled, or reissued after activation.
- Because Moment spending cannot be adjusted to exact zero-unit amounts, spending above the package amount is required.

### FAQ Rules

- Existing 2023/2024 package accounts must be recreated under the 2025+ revised guide; 2025 accounts may be reused.
- Package shortfall, even by a small amount, is not allowed.
- Agency commission is the same as ordinary Moment ad commission.
- CPT/guaranteed schedules follow the standard process, but execution and schedule must be shared for monitoring.
- If Gift exposure is in October, the Moment package period cannot include November. It must stay in the same month with the Gift exposure date.
- Package accounts are basically for package campaigns only. Non-package campaigns are not allowed even if they use Gift landing unless discussed with Kakao.

## Kakao Ad and Service Structure

- Kakao Moment and Channel Admin Center areas are checked through Kakao advertiser-side contacts.
- Seller Center and Seller Center message-sending areas are checked through Kakao Commerce CM.
- Kakao advertising assets sit under a Kakao account / Kakao Business email account.
- Advertising assets include ad accounts, Pixel & SDK, Business Wallet, etc.
- To link Pixel & SDK with an ad account or Kakao service, the Kakao account must be Pixel & SDK master/member and also ad account master/member or service master/manager.

### Message Sending Platforms

| Platform | Landing | Targeting | Responsible side | Permission |
|---|---|---|---|---|
| Kakao Moment | URL, post, coupon, AdView, KakaoTV, etc. | Gender, age, interest, region, friend group, ad-response target | Kakao advertiser contact | Master/member |
| Channel Admin Center | URL, post, coupon, AdView, KakaoTV, etc. | Gender, age, interest, region, friend group | Kakao advertiser contact | Master/manager |
| Seller Center: Shopping / Gift | Shopping, Gift, live, KakaoTV only | Gender, age, Seller Center-only purchase-history targeting, etc. | Kakao Commerce CM | Master/manager |

For Talk Channel and Moment, sending is possible when the Kakao account logged into the ad account is channel master/manager. Talk Store can send after seller-center connection. Gift channel connection requires Kakao CM mapping.

## Updates and Tips

### Commerce Gift / Talk Store Catalog Auto-linked Products: Placement Expansion

- Planned application: 2026-02-25.
- Applies only to products using catalog auto-linking.
- Placement selection is not available.
- Gift catalog can expose in Gift inventory.
- Gift/Talk Store catalog can expose in Shopping Tab inventory.

### Performance Ad Creative Frequency Detail Setting

- Applied: 2026-02-10.
- Available for performance ads: Bizboard/display conversion objective, visit objective, and video view objective.
- Frequency can be controlled by user exposure action, for 1-24 hours and 1-5 exposures.
- Use this to manage fatigue, but expect possible under-delivery if the audience is narrow.

### Commerce Gift / Talk Store Catalog Auto-linking

- Opened: 2026-01-14.
- Moment product catalog ads can run based on linked catalog products, recommending personalized products for purchase conversion.

### Message Catalog Type Beta

- Opened: 2025-12-08.
- One message can include up to 7 content items.
- Item types:
  - Discount emphasis type: visually emphasize high discount rate.
  - Price emphasis type: communicate reasonable price or limited coupon/card price.
  - Content emphasis type: introduce new products or branded content requiring explanation.

## Campaign Setting Change Strategy

When CTR decline, under-delivery, or ROAS decline continues during long-term Moment operation:

### Consolidate Similar Groups

- Avoid splitting very similar targets into many groups because internal competition and fragmented learning can hurt efficiency.
- Combine similar categories when appropriate.
- Split only when targets or creatives do not overlap.
- Combined conversions per group can help optimization-stage improvement.

### Creative Replacement and Soft Landing

- New creatives need learning and optimization time.
- When existing high-performing creative is still working, do not replace it aggressively.
- If existing creative efficiency drops significantly, switch it off and activate new creative.
- For many new creatives, use gradual replacement and A/B tests.

### Avoid Abrupt Changes

- Avoid sudden targeting changes that are too narrow or too broad.
- Avoid budget changes over 20%; use gradual changes.
- Avoid frequent on/off. Use time targeting where possible.
- Do not immediately stop a low-performing campaign after a short test; keep small stable spend when learning is still possible.

## Event Friend Message

Event friend message targets channel friends who clicked DA ads or triggered Pixel & SDK conversion events. It can send real-time customized messages without separate development.

### Targetable Events

| Event type | Send target | Detail |
|---|---|---|
| Click event | Channel friends who clicked ads under the ad account | All possible clicks or specific campaign clicks |
| Conversion event | Channel friends who triggered Pixel & SDK events linked with the ad account | All conversions or specific Pixel & SDK and event |

### Send Timing

Options: immediate, 3 minutes, 5 minutes, 10 minutes, 30 minutes, 1 hour, 3 hours, 1 day, 3 days, 5 days, 7 days after event.

Use immediate sending for instant action and delayed sending for reminders.

### Pricing

- Standard send price: KRW 50.
- CBT promotion price: KRW 40 regardless of type.
- Budget cap can be set.
- Remaining budget after end schedule can be used to send to high-response friends at KRW 20 or refunded immediately, according to the provided guide.

Critical caution: this targets channel friends, not all ad clickers.

## Ad-response Targeting

- Ad-response target creation takes about 1 hour.
- Default collection period is recent 90 days.
- If no users reacted during the period, there may be no exposure target.

### Display Ad Response

- Create targets from display ad click/open users.
- For Bizboard and video ads, video play data can be used.
- Users who clicked and converted from Kakao channel messages can be created under display ad-response target and used in display campaigns.

### Message Ad Response

- Create targets from message open, click, and video play users.

### Scenario Examples

| Situation | Target creation | Retargeting | Detargeting |
|---|---|---|---|
| Awareness/reach | All campaign click users | Repeat exposure to clicked users | Expand new users |
| Specific product/event interest | Specific product or promo campaign click users | Provide additional information | - |
| Purchase conversion | Click users minus conversion users | Send discount/coupon to non-converters | - |
| Message open improvement | Message open users | Send to high-open users | Use benefit-focused preview creative to long-term non-openers |
| Message click improvement | Message click users / video play users | Send to high-click users | Use benefit-focused creative to long-term non-clickers |
| Display to message converters | Message conversion users | Show repurchase benefit | Exclude purchasers for additional prospecting |

## Situation-based Proposal Scenarios

| Situation | Recommended mix | Scenario | Notes |
|---|---|---|---|
| New product / spot promotion | Bizboard CPT / Profile Full View | Secure strong time/day reach and create market presence | Full View for full-screen image/video; Bizboard CPT for time concentration |
| Purchase conversion maximization | Display x conversion / Bizboard x conversion / Product Catalog x conversion | Use display/Bizboard and dynamic catalog retargeting to drive purchase conversion | Better with Pixel & SDK seed events. Product catalog x conversion may be CBT; recheck availability |
| Signup or Talk Channel add conversion | Display x conversion / Bizboard x conversion | Optimize by signup Pixel event or KakaoTalk channel-add goal | Exclude existing signups/channel friends. CPA bidding may be available |
| Dormant-customer revisit | Display/Bizboard conversion objective + personalized message reach | Detarget previous visitors/purchasers from acquisition and send messages to dormant customers | Effective with revisit/repurchase benefits |
| Repurchase / loyalty | Display/Bizboard conversion objective + channel message or personalized message reach | Retarget purchasers, maintain high core-target reach, and send coupons/new product messages | If retargeting audience is too narrow, use no targeting or visit objective first |

If retargeting/conversion optimization seed is insufficient, run visit campaigns first to secure traffic.

## Budget Scenario

### By Target Size

| Target/budget shape | Objective | Strategy | Recommended products |
|---|---|---|---|
| Broad target + high budget | Awareness expansion | Use guaranteed products for strong reach | Profile Full View, Bizboard CPT |
| Broad target + low budget | Efficient reach | Mix guaranteed and performance products where realistic | Performance display/Bizboard; avoid over-fragmentation |
| Narrow target + high budget | Core target conversion | Use conversion optimization and reduce fatigue with creative variety | Conversion ads with frequency control |
| Narrow target + low budget | Efficient conversion | Use core targeting and conversion-focused reach | Custom targets/core targets, but beware under-delivery |

For limited budgets, expand placements including network inventory to secure lower-CPC traffic where appropriate. For narrow targets, too much budget can cause over-frequency and ROAS decline; frequency cap can help but may cause under-delivery.

### By Monthly Budget

| Monthly budget | Strategy | Recommended mix |
|---:|---|---|
| <= KRW 5M | Use efficient CPC display placements; network inventory may help | Display x visit / interest targeting |
| KRW 5M-15M | Run display and Bizboard together with category/interest targeting | Bizboard x visit + Display x visit |
| KRW 15M-30M | Secure at least KRW 500K/day always-on exposure and add periodic channel messages | Bizboard x visit, Bizboard x conversion, channel message |
| >= KRW 30M | Use multi-product placement mix for spot and always-on exposure | All applicable types |

For conversion objective, check whether Pixel & SDK has at least 1,000 learning events in the recent 30 days before relying on conversion optimization.

## Bidding Strategy

| Bid type | Auto bidding | Manual bidding |
|---|---|---|
| Operation | System adjusts bids based on group daily budget | Fixed bid entered by operator |
| Option | Cost target setting available | No cost target |
| Character | After about 10 minutes of learning, guides appropriate cost target and daily budget. ROAS target may be provided later | Lower risk of exceeding the fixed bid |
| Caution | Not suitable for short-term operation. New groups may need 2-3 hours for bid exploration. Works toward target over 2-4 weeks, not daily exact target | Suitable for short-term fixed-budget operation. Wrong bid can under-spend or over-spend |
| Available objectives | Visit, conversion | Visit |

If initial bid is hard to determine, use auto bidding first, then check average bid level and switch/reference manual bidding if needed.

Cost target works better when conversion volume is high and daily performance volatility is low. Use all placements including network inventory for better delivery and learning when appropriate.

## Conversion Optimization Tips

If first using conversion campaigns, set target/budget so the goal conversion can reach at least 50 conversions per 7 days.

Recommended daily budget formula:

> Daily budget = target daily conversions x expected CPA

Example: 10 conversions/day x KRW 20,000 CPA = KRW 200,000 daily budget.

For stable learning, secure at least 7 days of learning and KRW 500K-1M daily budget when possible.

### Setup Guidance

- Minimize campaigns and ad groups to avoid learning budget fragmentation.
- Loosen targeting and bid limits for smooth group learning.
- Start with a minimum number of creatives; manage on/off around high-performing creatives.

### Optimization Stage

| Status | Group conversions in 7 days | Meaning |
|---|---:|---|
| Stage 1 | <20 | Uses users who clicked creative category and converted as seed; 50+ conversions needed for stronger optimization |
| Stage 2 | 20-49 | Basic ML operates; more conversions needed |
| Stage 3 | 50-499 | Advanced ML operates; more conversions needed |
| Stage 4 | >=500 | Strongest ML operation |
| ML learning wait | - | After group creation or restart after long stop. Status change may take 4 hours, initial creation up to 8 hours |
| Not available | - | Pixel & SDK unlinked/deleted or temporary unavailable |

Even with low/no event seed, Kakao data and ML can extract likely converters, but more advertiser event data improves optimization.

If ad execution stops for more than 3 days, campaign may enter limited ML learning wait / cold start. Once conversion volume is sufficient, optimization can resume from the next day.

## Pixel & SDK Readiness

Pixel & SDK is Kakao's conversion tracking service. It tracks user actions and helps identify prospects and measure ad-driven signup/purchase conversions.

Pixel data should ideally be collected for 2-3 weeks before starting conversion ads.

If Pixel & SDK is not installed:

- Performance measurement is limited.
- Retargeting by page/action and purchaser detargeting are limited.
- Conversion optimization cannot use advertiser conversion data.

Pixel dashboard:

- `https://business.kakao.com/pixel/`
- Path: Business Admin Center -> Business tools -> Pixel & SDK -> Pixel & SDK name -> Dashboard -> Inflow route detail.
- Period can be set up to 31 days.
- Filter by event or inflow route; click graph to view detailed logs.

## ASAP Program

ASAP is a Kakao agency partner support program designed to help partner agencies achieve stable ad business and performance.

For 2026 Q2, details may change. Recheck by email before quoting externally:

- `partnerboost@kakaocorp.com`

Use ASAP as an internal enablement/support mechanism, not as a guaranteed advertiser benefit unless Kakao confirms eligibility.

## Client-facing Safe Wording

> 카카오는 단순 노출형 DA 매체가 아니라, 카카오톡 기반 생활 접점에서 고객을 발견하고 비즈니스폼, 카카오싱크, 톡채널, 메시지 광고를 통해 유입 이후의 관계 자산화를 설계할 수 있는 매체입니다. 다만 광고 클릭만으로 메시지 발송 권한이 생성되는 것은 아니므로, 가입, 채널 친구 추가, 마케팅 수신 동의, 픽셀&SDK 이벤트 등 단계별 조건을 확인한 뒤 리타겟팅과 메시지 재접촉 구조를 설계해야 합니다.

## Proposal Checklist

Before proposing Kakao Moment:

- Is the goal awareness, traffic, purchase, signup, channel add, lead collection, repurchase, or CRM?
- Does the advertiser have Pixel & SDK installed and enough recent events?
- Does the advertiser have Kakao channel assets, friend base, consent data, or Kakao Sync?
- Is the budget enough for the selected objective? For conversion, can it generate 50+ conversions in 7 days?
- Are campaign/ad group counts minimized enough for learning?
- Are similar targets consolidated?
- Are creative replacements gradual rather than disruptive?
- Will sudden budget changes over 20% be avoided?
- If using packages, has dedicated account, whitelisting, Gift landing URL, period, spend floor, and free-cash rule been confirmed?
- If using CBT/beta features, has current availability been checked with Kakao?
