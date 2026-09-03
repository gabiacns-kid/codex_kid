# Toss Ads Basic Operation Guide

Use this reference when preparing Toss Ads proposals, media mix expansion ideas, reward/offerwall advertising plans, traffic boosting, promotion/new-product/live-shopping/CPA participation campaigns, or Toss Ads account/operation guidance.

Official sources checked:

- https://toss-ads.gitbook.io/guide
- https://toss-ads.gitbook.io/guide/policy
- https://toss-ads.gitbook.io/guide/a-d/banner
- https://toss-ads.gitbook.io/guide/a-d/banner/objective
- https://toss-ads.gitbook.io/guide/a-d/banner/creative
- https://toss-ads.gitbook.io/guide/a-d/money-notifications
- https://toss-ads.gitbook.io/guide/a-d/luckyquiz
- https://toss-ads.gitbook.io/guide/a-d/liveshopping
- https://toss-ads.gitbook.io/guide/a-d/shortform
- https://toss-ads.gitbook.io/guide/a-d/buttonpress
- https://toss-ads.gitbook.io/guide/a-d/catalog_vote
- https://toss-ads.gitbook.io/guide/a-d/weeklymission
- https://toss-ads.gitbook.io/guide/a-d/visitmission
- https://toss-ads.gitbook.io/guide/resources/tag
- https://toss-ads.gitbook.io/guide/resources/mat
- https://toss-ads.gitbook.io/guide/resources/tosspixel
- https://toss-ads.gitbook.io/guide/resources/target
- https://toss-ads.gitbook.io/guide/adjustment/ad_money
- https://toss-ads.gitbook.io/guide/adjustment/settlement
- https://toss-ads.gitbook.io/guide/adjustment/penaltyguide

Note: the provided webhook URL `https://toss-ads.gitbook.io/guide/resources/webhook` did not load during the check. Treat webhook integration as a confirmation item until the page or official material is accessible.

## GabiaCNS Positioning

Toss Ads should usually be treated as an **additional media expansion option**, not the default primary performance channel.

Recommend Toss Ads when the advertiser needs:

- Promotion burst.
- New product awareness and traffic.
- Live shopping traffic boosting.
- Reward/participation-based CPA or action campaigns.
- Extra media mix reach beyond Naver, Kakao, Meta, and Google.
- High-attention exposure through Toss app benefit surfaces and financial/consumption context.

Do not over-frame Toss Ads as a stable ROAS channel by default. Many products use reward, quiz, mission, or offerwall-like mechanics, so cherry-picker participation and post-click quality must be discussed.

Client-facing wording:

> 토스 광고는 네이버·카카오·메타·구글을 대체하는 기본 성과 매체라기보다, 토스의 높은 앱 사용성과 혜택탭 기반 주목도를 활용해 프로모션, 신제품, 라이브방송, 참여형 CPA 목적을 보완하는 확장 매체로 보는 것이 적합합니다. 다만 리워드형 구조상 참여량은 빠르게 만들 수 있어도 실제 구매·잔존·리드 품질은 별도 검증이 필요합니다.

## Account and Operation Structure

Toss Ads uses business groups and ad accounts.

- A business group can contain multiple ad accounts, useful for agencies managing multiple brands.
- The business group is the tax invoice issuance basis through its business registration number.
- Ad spend settlement is calculated by ad account.
- Group owners can approve ad account creation and view group ad account spend/operation status.
- To run ads, a user must be invited to the ad account; ad account participation cannot be directly requested in the guide.
- Ad account transfer is listed as a supported start-guide topic; confirm exact current transfer steps before client handoff.

Agency implication:

- For agency onboarding, confirm business group ownership, ad account access, representative email, tax invoice needs, and whether the account is prepaid or postpaid.
- If taking over an existing advertiser, verify transfer/access rights before promising a start date.

## Product Map

### Banner Ads

Role:

- Flexible display product for traffic, reach, lead collection, and teen awareness goals.

Campaign objectives found in the guide:

- Visit: optimize for clicks and landing visits.
- Reach: reduce duplicate exposure and reach more users; supports payment-history based targeting in self-serve targeting.
- Lead collection: uses question forms to collect prospect answers; downloaded lead data is available for 30 days from lead occurrence.
- Teen awareness: targets users aged 14 to 18 for brand awareness.

Creative/operation notes:

- Creative review works by all-review or individual-creative review.
- Draft campaigns are auto-saved for 14 days.
- Campaigns can have up to 100 ad sets and each ad set up to 100 creatives in the checked guide.
- Ad set/creative ON/OFF operation is available; off creatives are not charged.
- Approved creatives cannot be deleted.
- Creative review operates on weekdays 10:00-19:00, and submission 2-3 business days before execution is recommended.
- Copy must be at least 5 Korean characters, avoid informal speech, excessive emphasis, repeated special characters, and Toss-like official UI confusion.
- Benefits shown in creatives must be verifiable on the landing page; inaccessible or pre-open landing pages can be rejected.

Proposal use:

- Use for traffic/reach/lead collection when the advertiser has landing readiness and tracking.
- For lead collection, warn that consent copy and personal data handling are advertiser responsibility.

### Money Notification

Role:

- Message-style ad to Toss money notification subscribers or card-notification/payment-context users.
- Strong fit for timely action, live-commerce start reminders, and consumption-context targeting.

Types:

- General: sends to target users based on recent consumption history.
- Live: sends when a live broadcast starts.
- Keyword: sends around selected payment-keyword contexts.

Key operating conditions from the guide:

- General/live can choose new target setup or existing target.
- Basic CPP is KRW 30 in the checked guide.
- Target condition additions can add KRW 10 each, up to KRW 100; age, gender, region, and device targeting do not add surcharge.
- Minimum target size is 30,000 people.
- Same-day execution is unavailable.
- Reservation time is 09:00-21:00.
- If the advertiser's server is small, 5,000 sends per minute is recommended.
- Keyword type budget is VAT excluded and starts from KRW 1,000,000.
- Keyword type exposure period is monthly.
- Keyword type targeting is limited to age and gender.
- Keywords: minimum 5 and maximum 20; at least 3 keywords from the provided keyword list are required.
- Keyword-type messages can be sent within 5 minutes after payment to card-notification opt-in users, and non-opt-in users can receive messages if they had matching payment history within the prior 7 days; duplicate messages can happen for multiple keyword payments.

Proposal use:

- Use for timely conversion prompts, live broadcast traffic, retail/finance/local-service payment-context campaigns.
- Push back when the advertiser cannot handle traffic or when landing/server is weak.

### Lucky Quiz

Role:

- Benefit-tab quiz product for large traffic and branding.
- Non-target product.

Key conditions:

- Cost can be selected from KRW 1,000,000 to KRW 20,000,000 in the checked guide.
- Cost selection changes exposure time and expected quiz participants.
- Not suitable when adult-only targeting is required, because it is non-targeted.
- Real-time concurrent access can exceed 150,000 per minute; landing URLs must handle short-term traffic spikes.

Proposal use:

- Use for burst traffic, brand recall, search/landing event participation.
- Avoid for adult-restricted or fragile landing/server environments.

### Live Market

Role:

- Live shopping traffic boosting through benefit-tab live exposure.
- Non-target product.

Types and benchmark traffic:

- Basic: benchmark 50,000 traffic.
- Plus: benchmark 150,000-200,000 traffic.
- Premium: benchmark 270,000 traffic.

Operating conditions:

- Basic broadcast duration: 20 minutes to 1 hour, 20-minute units.
- Plus: 30 minutes to 1 hour, 10-minute units.
- Premium: 1 hour to 6 hours, 30-minute units.
- Listing starts 24 hours before the live broadcast and users receive pre-notifications.
- Same-day booking makes efficiency hard to guarantee.
- Adult-only targeting is difficult because it is non-target.

Proposal use:

- Use when the advertiser has live inventory, host/content readiness, benefits, and stock/server capacity.

### Shortform

Role:

- Live Market shortform-style video exposure with directly assigned boosting time.
- Non-target product.

Operating notes:

- Start time is the video boosting time.
- Toss app detail information appears from 24 hours before start time.
- Adult-only targeting is difficult.

Proposal use:

- Use when video assets and commerce offer are strong.
- Avoid promising sales uplift without checking product, price, video quality, landing, and stock.

### Button Press

Role:

- Reward/CTA button product in the Toss benefit tab.
- Good for low-cost user acquisition and high traffic.

Key conditions:

- Benefit-tab banner exposure; clicking shows a CTA button to earn points, then can move to brand landing page.
- Submit creative review 2-3 business days before execution.
- Execution dates are day-based.
- Weekday exposure: 19:00-23:59.
- Weekend exposure: Saturday/Sunday 00:00-17:59 in the checked guide.

Proposal use:

- Use for traffic and simple participation, but warn about reward-driven traffic quality.

### Catalog Vote: "두근두근 1등 찍기"

Role:

- Catalog/vote participation product that exposes multiple SKUs and asks users custom questions up to twice a day.
- Designed to maximize engagement with low CPC and large traffic potential.

Key conditions:

- Day-based date selection.
- Execution date can be selected only up to at least 1 business day before execution.
- Campaign name up to 20 characters.
- Once selected, the execution date cannot be changed.
- Campaign cancellation/refund follows penalty policy.
- Creative review is required; creatives in review/scheduled/approved status cannot be edited.
- Non-target product, so adult-only targeting is difficult.

Proposal use:

- Use for product preference checks, SKU awareness, new product feedback, and traffic.

### Today's Point Mission / Weekly Mission

The URL provided is "오늘의 포인트 미션," but the loaded guide page title is "이번 주 미션." Use the official page title when writing client-facing docs unless a newer naming source confirms otherwise.

Role:

- Offerwall product that rewards users for ad participation.
- Supports KPI-oriented actions such as signup, app launch, purchase, event participation, SNS promotion.

Key conditions:

- Targeting can include gender, age, OS, SDK, tracking permission, and similar conditions.
- Charges only when actual conversion/action occurs according to the guide.
- Benefit-tab main page list exposure; more than 10 cards with age-specific missions can appear.
- After users enter advertiser page and complete mission, points are paid within 3 minutes.
- Unit price and minimum execution standards are discussed with NBT; contact point in guide: `toss_adison@nbt.com`.
- Some product types may not be visible without product signing; confirm with NBT.

Proposal use:

- Use for CPA/action campaigns, app installs/execution, signup, purchase/event participation.
- Must warn about cherry-picker risk, deduction/reconciliation rules, and valid-action definition.

### Visit Mission

Role:

- Beta product to drive repeated visits to online mall home, event, product web/app pages from Toss users active in finance/consumption.

Key conditions:

- Bookable in 7-day units.
- Depending on budget, guide says up to 1M+ daily inflow can be expected.
- Beta product; inquiry through `reward.mission@toss.im`.

Proposal use:

- Use for shopping mall/store awareness and visit boosting.
- Confirm beta availability, cost, and eligibility before proposal.

## Tracking and Assets

### Conversion and Tracking

The guide contains sections for:

- Conversion tracking code creation.
- Conversion tracking code sharing/transfer.
- Conversion events.
- Conversion tracking/integration status.

Confirm details before implementation because the top-level page mostly routes to subpages.

### App MAT Integration

Supported MAT guide sections:

- Adjust.
- AppsFlyer.
- Airbridge.
- DFINERY.
- Branch.
- Singular.

Use MAT integration when app install, app open, in-app action, or CPA action validation matters.

### Toss Pixel

Role:

- Web campaign conversion event collection.

Support/limits:

- Supports self-mall, Cafe24, and MakeShop in the checked guide.
- Browser API based SDK; does not work in native app environments.

Events:

- pageView.
- signUp.
- productView.
- addToCart.
- purchase.
- lead.
- customevent.

Parameter principle:

- Events can fire without optional parameters, but richer parameters improve analysis precision.
- currency must use ISO 4217 format, such as KRW or USD.

Proposal use:

- For web commerce campaigns, include Toss Pixel readiness before promising conversion optimization.
- For app campaigns, use MAT rather than Toss Pixel.

### Target and Audience

Top-level target guide sections:

- Ad-response target.
- Conversion-tracking target.
- Customer-list target.
- Target-combination feature.

Use this as a retargeting/audience expansion readiness area, but confirm exact eligibility and privacy requirements before delivery.

### Webhook for Lead Collection

The provided webhook URL did not load during this check. Confirm official webhook setup before promising lead integration.

## Billing, Settlement, and Penalty

### Ad Money / Business Wallet

Important update:

- From April 2026, the guide says the ad cost management system moves to Business Wallet.
- Existing ad money becomes business money, with sequential migration.

Ad money types:

- Paid money: charged by card or virtual account.
- Free money: promotional/event money from Toss; expires automatically and is spent first when nearer to expiration.
- Postpaid accounts can run without separately charging paid money and settle in bulk early next month within postpaid limits.

Operational cautions:

- If auto-charge is disabled and money is exhausted, running ads stop automatically.
- Valid clicks/execution during stop-reflection timing can create negative balance.
- Auto-charge card registration requires account-owner authority.
- One card per ad account.
- Auto-charge condition can be set from 10,000 KRW or less to 500,000 KRW or less.
- Auto-charge amount can be 100,000-5,000,000 KRW; direct input cannot exceed a daily max of 10,000,000 KRW in the checked guide.

### Settlement

- Settlement statement is created on the first day of the next month based on paid ad money spent for ads actually executed from the first to the last day of each month.
- Tax invoices are issued monthly based on paid money spent.
- Tax invoice issuance basis is ad-account level; some agency accounts may issue one invoice by business registration number after prior consultation.
- Free ad money usage is not included in the tax invoice.

### Penalty

General:

- Cancellation penalties depend on cancellation timing and product.
- Timing uses business days, excluding weekends and holidays.
- Penalty basis is booked campaign, not creative submission.
- Penalties are immediately deducted from paid money; postpaid accounts must deposit by the end of the following month.
- Cancellation penalties are not tax-invoice targets and agency commission is not paid on penalty amounts.

Selected product rules from the guide:

- DA banner: no penalty if no actual spend occurred.
- Money Notification: 20%, 50%, or 100% depending on timing.
- Live Market, Shortform, Lucky Quiz: 50% or 100% in closer cancellation windows.
- Button Press and Catalog Vote have separate 2025-05-01 onward rules: 10%, 20%, 50%, 100% style timing windows; Catalog Vote cannot be canceled from 23:00 the day before execution in the checked guide.

Proposal caution:

- For booked products, confirm dates and creative readiness before booking.
- Always mention penalty policy before campaign creation where product pages require agreement.

## Strategy Selection

Use Toss Ads as a purpose-led add-on:

| Objective | Recommended Toss Ads fit | Caution |
|---|---|---|
| Broad traffic/awareness | Banner, Lucky Quiz, Button Press | Reward or curiosity traffic may be low intent |
| Promotion burst | Lucky Quiz, Money Notification, Button Press, Catalog Vote | Landing/server readiness required |
| Live broadcast traffic | Live Market, Money Notification Live, Shortform | Booking lead time and live benefits matter |
| New product/SKU interest | Catalog Vote, Banner, Lucky Quiz | Vote/traffic does not equal purchase intent |
| CPA/action | Weekly Mission, MAT/pixel-supported campaigns | Valid action definition and cherry-picker quality must be managed |
| Shopping visit boost | Visit Mission beta, Button Press, Banner | Beta availability and retention quality check |
| Retargeting/audience use | Banner with target/audience, Toss Pixel/MAT | Tracking setup required |

## Risks and Critical Pushback

- Reward and offerwall structures can create cherry-picker traffic.
- High traffic does not automatically mean high purchase quality.
- Non-target products are unsuitable for adult-only or heavily restricted targeting needs.
- Landing pages, servers, live commerce pages, and event pages must handle short traffic spikes.
- Conversion tracking must be set before performance claims.
- CPA products require valid action definitions, duplicate/fraud handling, and reconciliation rules.
- Cancellation/booking penalties can be material; do not book casually before creative and schedule are firm.
- Toss Ads is best framed as an extension layer alongside Naver/Kakao/Meta/Google, not as a replacement for core acquisition media.

## GabiaCNS Proposal Wording

> 토스 광고는 혜택탭과 리워드형 참여 구조를 활용해 단기간 트래픽, 프로모션 참여, 라이브방송 유입, CPA 액션을 만들기 좋은 확장 매체입니다. 다만 리워드 기반 유저 유입은 실제 구매 의도와 차이가 있을 수 있어, 가비아CNS는 캠페인 목적을 먼저 분리하고 랜딩·서버·트래킹·유효 액션 기준을 확인한 뒤 네이버·카카오·메타·구글 외 보조 확장 매체로 제안하는 방식을 권장합니다.

## Confirmation Checklist Before Proposal

- Current product name and availability.
- Current minimum budget, cost basis, VAT inclusion/exclusion.
- Targeting availability: targeted vs non-targeted.
- Adult/restricted category eligibility.
- Creative review lead time.
- Booking and cancellation penalty window.
- Landing/server traffic capacity.
- Pixel/MAT/conversion tracking readiness.
- Valid action and deduction/reconciliation criteria for CPA/offerwall products.
- Agency account/transfer/access and settlement structure.
