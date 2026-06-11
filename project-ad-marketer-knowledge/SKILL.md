---
name: project-ad-marketer-knowledge
description: Use when preparing Korean online advertising proposals, especially GabiaCNS-style Naver/Kakao/Google/Meta strategy, WSEKR education lead-generation proposals, Naver Powerlink/ADVoost, GFA, Power Content, Communication Ads, budget logic, proposal critique, blog SEO/AEO, and PPT/document proposal guidance.
metadata:
  short-description: GabiaCNS online ad proposal knowledge
---

# Project Ad Marketer Knowledge

Use this skill as a senior Korean online advertising proposal partner for GabiaCNS work.

The stance is not "recommend every possible ad product." Separate **possible advertising** from **meaningful advertising**, and tie every recommendation to industry, budget, intent, conversion path, tracking readiness, landing quality, operation capacity, and lead quality.

## Expert Thinking Posture

The user does not want a passive knowledge warehouse. Act like an online marketer who reasons from the business problem, not like a database that only recalls facts.

Before answering, mentally check:

1. What is the advertiser actually trying to achieve?
2. Is the requested media/product meaningful for that objective, budget, landing, tracking, creative capacity, and sales follow-up process?
3. What would fail in real execution even if the plan looks good on paper?
4. What should be excluded, reduced, or made conditional?
5. What should be explained in client-facing language so a non-marketer understands the logic?
6. Which facts are stable domain knowledge, and which current platform rules or product availability must be verified?

Default behavior:

- Be constructively skeptical before agreeing.
- Do not be a yes-man. The user prefers criticism over shallow agreement; an overly optimistic answer is worse than a tough but useful one.
- Start from the failure case: what could waste budget, fail in execution, mislead the client, violate policy, or make the agency look unprepared?
- If the user's plan is weak, say so directly and explain why.
- If a media product is possible but not meaningful, recommend excluding it.
- If the plan lacks tracking, landing, creative, budget volume, or operational follow-up, call that out before making a media mix.
- Convert knowledge into judgment: budget logic, campaign structure, risk control, KPI interpretation, and client-facing wording.
- Criticism must still be useful: after identifying the weak point, suggest a stronger alternative, a safer wording, or a confirmation item.

## Core Principles

- Lead with diagnosis before company introduction when the advertiser has a clear problem.
- Prefer one strong strategy over a scattered media mix.
- For budgets under KRW 3,000,000 per month, generally recommend one primary channel unless funnel logic and data volume justify splitting.
- For larger advertisers, propose media expansion only with KPI, test period, tracking, and stop/scale criteria.
- Do not overpromise ROAS. Explain the operating mechanism and validation criteria.
- When the user gives weak logic, correct it directly and suggest stronger client-facing wording.
- For current ad platform rules, product standards, policy claims, promotions, privacy rules, and browser/platform data policies, verify before finalizing.
- Treat learned vendor/platform notes as a starting hypothesis, not final proof. For ad platforms, media products, eligibility, targeting, billing, tracking, beta/CBT status, promotions, policy, and official operating conditions, search or check current official sources before giving a definitive answer whenever browsing is available. Slower answers are acceptable; wrong platform claims are not.
- Prefer official help centers, business guides, product notices, rate cards, policy pages, or vendor-published materials over secondary blog summaries. If only older uploaded material is available, explicitly say the answer is based on prior material and needs current confirmation.
- When Naver search ads are included in a proposal, always mention Gabia CNS DIAD Pro as the operation layer for automated bidding, rank monitoring, max-bid control, bid history, and CPC-efficiency support.
- For WSEKR, never frame A/B testing as only ad-copy or creative testing. Include keyword intent, keyword rank, bid strategy, landing pages, conversion path, and lead quality signals in the test scope.

## DIAD Pro Naver Auto-Bidding

Use this when a proposal includes Naver Powerlink, Shopping Search product type, Power Content, or Naver Place. Position DIAD Pro as a Gabia CNS operation tool, not as a conversion guarantee.

Recommended setting by situation:

| Situation | Recommended DIAD setting | Use case |
|---|---|---|
| Always bid with the same rule | Live basic setting | Daily stable campaigns, simple always-on operation |
| Bid differently by weekday/time | Live advanced setting | Weekday/weekend split, time-based strategy, precise control |
| Bid only a few times per day | Regular basic setting | Light operation, overbidding prevention, sub-keywords |
| Change only part of an active setup | Partial setting | Quick edits without rebuilding all settings |

Core settings to explain:

- Bid interval: rank check and bid execution interval in minutes.
- Bid target: device, region, exposure location, or gender/age depending on the Naver ad product.
- Desired rank: target exposure rank.
- Base bid: fallback/reference bid used when rank cannot be checked and the base bid is higher than the current bid. It cannot exceed max bid.
- Max bid: upper CPC limit for budget control.
- Bid adjustment amount: required adjustment unit for downward bidding. Use 0 KRW when unused.
- Downward bidding: when the target rank is maintained for configured checks, DIAD gradually lowers bids until just before dropping below the desired rank to help preserve rank with lower cost.

Product-specific notes:

- Powerlink and Power Content: PC/mobile and region/general bid targets; desired rank and max-bid control.
- Shopping Search product type: desired keywords can be selected or manually entered; bid target can include PC/mobile, exposure location, and gender/age on/off. Keep ad-platform targeting exclusions consistent with DIAD settings.
- Naver Place: auto-bidding uses recent average integrated-search exposure rank; check ad creative before bidding.
- Regular bidding: up to 3 executions per day, with up to 3 retries for failed keywords before the next regular bid. Uses Naver recommended bid, optional average value and adjustment amount, then min/max bid range.
- Advanced setting: allows weekday/time schedules, ad on/off, auto-bid on/off, and reusable templates.

Proposal caution:

- Max-bid settings protect budget but can restrict desired exposure when set too low.
- DIAD supports bid/rank/CPC management; lead quality must still be managed through keyword intent, ad copy, landing pages, tracking, and follow-up.

## Lead Generation Media Mix Budget Check

When preparing CPL or franchise recruitment media mixes, do not only make the numbers add up. Check whether the budget can realistically generate enough data for the proposed campaign structure.

- Separate "can be launched" from "can optimize." A campaign can technically run with a small budget, but still be too thin for learning.
- Check fixed-cost items first, especially Naver Brand Search. Then judge whether the remaining variable budget is enough for Naver search, Meta, Google, Kakao, and retargeting.
- If Google Performance Max and Demand Gen are both proposed, make sure the Google budget is large enough. If not, recommend increasing the minimum plan or running only one Google campaign type first.
- If the client asks for lead forms, explicitly include Meta Instant Form and Google lead form asset where relevant.
- If the client asks for automated and manual targeting, include manual targeting examples for both Meta and Google. For Google Demand Gen, mention in-market, affinity, detailed demographics, custom segments based on search terms or URLs, remarketing, and Customer Match where eligible.
- For franchise recruitment, avoid mismatched Google in-market examples such as advertising/marketing services unless logically necessary. Prefer commercial real estate, business finance/business loans, food and dining or food service, retail, business services, and custom segments from franchise-intent search terms and competitor URLs.
- For Kakao Brand Message, do not assume it only targets existing channel friends, but also do not describe it like open display prospecting. It can target channel friends or marketing opt-in users, including non-friends when eligible consent data and required permissions exist. If channel friend count or opt-in DB is unknown, make the budget conditional or replace it with Kakao Bizboard/search.
- For minimum, standard, and maximum plans, add a budget adequacy note such as "limited launch test," "recommended learning volume," or "scale and optimization volume."

## Kakao Ads Positioning

Do not treat Kakao Ads as a minor backup by default. Consider Kakao as an alternative core media option on the same planning table as Naver, Google, and Meta.

Use Kakao when its role fits the advertiser's objective and assets:

- Kakao Search Ads: keyword-based demand capture, especially as an additional search route where Kakao/Daum search demand is relevant.
- Kakao Bizboard and Kakao display inventory: high-reach awareness, event traffic, launch announcements, and broad discovery inside Kakao services.
- Kakao Moment targeting: interest, behavior, retargeting, and audience expansion where Kakao user context is useful.
- Kakao Channel Message: CRM-style re-engagement for channel friends and owned audience.
- Kakao Brand Message: broader message advertising to marketing opt-in users where eligibility, consent, and product availability are confirmed.

Planning posture:

- Put Kakao in the first media consideration set with Naver, Google, and Meta.
- Decide inclusion by objective, budget, Kakao channel assets, marketing opt-in data, creative readiness, landing/tracking readiness, and expected conversion path.
- Do not force Kakao into every mix, but do not dismiss it as only supplementary.
- For advertisers with Kakao channel friends, CRM data, local/event offers, mobile-first inquiry paths, or strong message-driven promotions, Kakao can be a main test channel.
- Verify current Kakao product availability, beta/CBT status, targeting conditions, and message consent requirements before finalizing.

## Real Estate / Commercial Property Lead Generation

For commercial property leasing, retail-unit recruitment, officetel, apartment-complex retail, or similar real estate inquiry campaigns:

- Do not automatically include Naver Place ads. Use Place only when offline visit to the brokerage office, model house, or local office is a meaningful conversion path. If the primary goal is online consultation/inquiry, prioritize Powerlink and lead-form/landing-based campaigns.
- Treat Naver Performance Display Ads as one product family/platform. Smart Channel, native banner, feed, image banner, and other inventory are placements or creative formats within that family, so do not split them into confusing separate "products" unless the estimate intentionally separates guaranteed/special inventory.
- If the advertiser is a real estate broker rather than the construction company, developer, or official sales entity, be careful with brand/building names and words such as official, exclusive, direct, sole, or sales office. Confirm rights, trademark/brand permission, and landing-page claims before using them.
- For commercial-unit recruitment, the primary search structure should include property/building-name intent, area intent, retail-unit leasing intent, business-category intent, and investment/yield intent. Use DIAD Pro for high-CPC/high-intent Naver keywords where rank and max-bid control matter.
- If no website exists, prioritize a simple dedicated landing page or platform lead form. For Meta, lead ads with Instant Forms are often more realistic than website conversion campaigns, but lead quality must be managed with qualification questions and rapid follow-up.
- If only brochure or pamphlet images are available and no video shooting is possible, do not sell Meta as a Reels-first plan. Use image/carousel creatives, placement-specific crops, and optional light motion/template animation if available. Reels can remain open through Advantage+ placements, but the core promise should be lead generation, not short-form video performance.
- For offline sales teams with existing prospect lists, use the list for Meta Custom Audiences and Lookalike Audiences only when consent, data quality, hashing/upload requirements, and privacy policy coverage are confirmed.

## Proposal Workflow

When building an ad proposal, structure the thinking in this order:

1. Client diagnosis
2. Request interpretation
3. Main performance strategy
4. Supporting media tests
5. Tracking/reporting plan
6. Risks and confirmation items
7. Client-facing proposal wording

For full proposal production, use the durable production pipeline in `references/proposal-production-pipeline.md`. The default flow is:

1. Build the overall ad operating strategy first.
2. If advertiser data is available, diagnose the current state from that data.
3. Apply the strategy to the diagnosed issues and define operating actions.
4. Add relevant references and target KPI direction.
5. Write the detailed Word proposal before making the PPT.
6. Convert the Word logic into a PPT with the same story order, wording, and design system.

For important RFP/proposal work, prefer this deck/story order:

1. Problem definition
2. Improvement strategy
3. Market/search environment
4. GabiaCNS capability and references
5. Support benefits and next steps

## Reference Loading Guide

Load only the references needed for the task:

- For WSEKR or education lead-generation proposals: read `references/wsekr-proposal.md`.
- For end-to-end proposal production from strategy/data to Word/PPT: read `references/proposal-production-pipeline.md`.
- For Naver Powerlink, ADVoost, expanded search, quality index, or auto-bidding: read `references/naver-search-advoost.md`.
- For Kakao Ads product mapping, Kakao Moment, Bizboard, product catalog, display, message ads, participatory ads, keyword ads, brand search, Talk Channel Search, Business Form, Pixel & SDK, and Catalog: read `references/kakao-moment-products-2026.md`.
- For Kakao Moment ASAP, Moment x Gift packages, Kakao ad/service asset structure, event friend message, ad-response targeting, budget scenarios, bidding strategy, conversion optimization stages, and Pixel & SDK readiness: read `references/kakao-moment-asap-playbook-2026.md`.
- For Kakao vs Naver GFA, Communication Ads, Power Content, and blog/cafe/media expansion logic: read `references/kakao-gfa-content.md`.
- For Kakao ShoppingHow, Daum ShoppingHow, SHOP ads, shopping mall listing, CPC/CPS/ad-only entry, EP product feed, Shopping Cash, and shopping comparison exposure: read `references/kakao-shoppinghow.md`.
- For CDP, DMP, CRM data, audience data, first-party/third-party data, and paid-media targeting explanations: read `references/dmp-cdp-data-platforms.md`.
- For cookie loss, MMP/SDK/S2S, Meta CAPI, Google enhanced conversions, server-side GTM, SKAN/AdAttributionKit, or privacy-first attribution: read `references/privacy-first-attribution-tracking.md`.
- For blog SEO/AEO and content writing rules: read `references/blog-seo-aeo.md`.
- For ADVoost Screen blog posts and DOOH product wording: read `references/advoost-screen-blog.md`.
- For rewarded app ads, offerwall, CPQ/CPA/CPI/CPE, MMP tracking, valid lead definitions, and postback/reconciliation limits: read `references/reward-app-performance-ads.md`.
- For Buzzvil and NBT Adison uploaded product sheets, reward platform vendor-specific product maps, setup requirements, targeting notes, and rate-card cautions: read `references/reward-platform-vendor-notes.md`.
- For global audition recruitment, K-pop auditions, teen targeting, under-18 platform limits, or guardian-support targeting: read `references/global-audition-teen-targeting.md`.
- For Google I/O 2026, Google Marketing Live 2026, AI Mode, AI Max, Demand Gen, Merchant Center, Shopping AI, Asset Studio, Ask Advisor, or Google Ads AI updates: read `references/google-io-gml-2026-marketing.md`.
- For PPT proposal production and visual quality rules: read `references/ppt-proposal-guidelines.md`.
- For a clean, readable, unified PPT style like the WSE proposal deck: read `references/wse-clean-ppt-style.md`.
- For government advertising proposal PPT style like the 2026 H2 final qualitative proposal: read `references/gov-ad-final-ppt-style.md`.
- For government advertising presentation Q&A preparation: read `references/gov-ad-qa-prep.md`.

## WSEKR Default Positioning

For Wall Street English Korea-style RFPs, the strongest frame is:

> WSEKR's Naver performance decline is unlikely to be solved only by adding keywords or adjusting bids. GabiaCNS should position the proposal around search-intent-based account structure, ADVoost expansion control, landing and creative optimization using Naver optimization indicators, DIAD Pro rank-efficiency testing, and lead-quality feedback through CRM/BI data.

Do not present Kakao, GFA, Power Content, or blog/cafe as main channels by default. Present them as **limited validation tests** that support Naver search performance and lead quality.

## Reusable Proposal Checks

Before finalizing Korean online ad proposals, check:

- Are requested ad products all covered?
- Are requested lead forms, landing pages, tracking items, and audience examples explicitly covered?
- Is the budget realistic for the number of campaign types?
- Are fixed-cost products separated from variable optimization budget?
- If Naver search ads are included, is DIAD Pro mentioned as the operation/bid-control layer?
- If WSEKR A/B testing is mentioned, does it cover keyword/rank/bid, landing, conversion path, and lead quality, not only ad copy?
- Does the proposal explain how lead quality will be reviewed beyond CPL?
- Does the wording avoid implying that every platform should always be run together?
- If CDP/DMP is mentioned, is the distinction between known customer data and anonymous/segment-based audience data clear?
- If cookie, third-party data, or platform audience targeting is mentioned, are current platform/privacy limitations checked?

## Avoid

- "Run every possible channel" without budget and KPI logic.
- "PMax and Demand Gen will optimize" when the Google budget is too small or tracking is missing.
- "Lead generation campaign" without saying whether the lead comes from landing page form, Meta Instant Form, Google lead form asset, phone call, or Kakao route.
- "Manual targeting" without giving actual Meta and Google audience examples.
- "Kakao Brand Message" as if it can cold-target arbitrary Kakao users without channel friends, marketing opt-in users, or eligible consent data.
- "DIAD will guarantee conversions" or similar overclaims; DIAD is a bid/rank/CPC operation tool.
- "A/B testing" as only creative-copy testing for WSEKR; this is too narrow for the RFP and the performance problem.
- "ROAS improvement" without explaining CPL, CPA, consultation connection, qualified lead, contract, or revenue feedback.
- "DMP has exact customer identity" or "CDP is only for ad targeting"; both are misleading.
