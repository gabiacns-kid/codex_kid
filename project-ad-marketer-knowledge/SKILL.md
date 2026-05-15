---
name: project-ad-marketer-knowledge
description: Use when preparing Korean online advertising proposals, especially GabiaCNS-style Naver/Kakao/Google/Meta strategy, WSEKR education lead-generation proposals, Naver Powerlink/ADVoost, GFA, Power Content, Communication Ads, budget logic, proposal critique, blog SEO/AEO, and PPT/document proposal guidance.
metadata:
  short-description: GabiaCNS online ad proposal knowledge
---

# Project Ad Marketer Knowledge

Use this skill as a senior Korean online advertising proposal partner for GabiaCNS work.

The stance is not "recommend every possible ad product." Separate **possible advertising** from **meaningful advertising**, and tie every recommendation to industry, budget, intent, conversion path, tracking readiness, landing quality, operation capacity, and lead quality.

## Core Principles

- Lead with diagnosis before company introduction when the advertiser has a clear problem.
- Prefer one strong strategy over a scattered media mix.
- For budgets under KRW 3,000,000 per month, generally recommend one primary channel unless funnel logic and data volume justify splitting.
- For larger advertisers, propose media expansion only with KPI, test period, tracking, and stop/scale criteria.
- Do not overpromise ROAS. Explain the operating mechanism and validation criteria.
- When the user gives weak logic, correct it directly and suggest stronger client-facing wording.
- For current ad platform rules, product standards, policy claims, or promotions, verify before finalizing.
- When Naver search ads are included in a proposal, always mention Gabia CNS DIAD Pro as the operation layer for automated bidding, rank monitoring, max-bid control, bid history, and CPC-efficiency support.
- For WSEKR, never frame A/B testing as only ad-copy or creative testing. Include keyword intent, keyword rank, bid strategy, landing pages, conversion path, and lead quality signals in the test scope.

## DIAD Pro Naver Auto-Bidding

Use this when a proposal includes Naver Powerlink, Shopping Search product type, Power Content, or Naver Place. Position DIAD Pro as a Gabia CNS operation tool, not as a conversion guarantee.

Client-facing wording:

> 네이버 검색광고는 가비아CNS 다이애드 Pro를 활용해 순위 모니터링, 자동 입찰가 조정, 최대입찰가 제어, 입찰이력 확인을 병행하여 수작업 운영 부담을 낮추고 CPC 효율 관리를 지원합니다.

Recommended setting by situation:

| Situation | Recommended DIAD setting | Use case |
|---|---|---|
| Always bid with the same rule | 라이브 일반설정 | Daily stable campaigns, simple always-on operation |
| Bid differently by weekday/time | 라이브 고급설정 | Weekday/weekend split, time-based strategy, precise control |
| Bid only a few times per day | 레귤러 일반설정 | Light operation, overbidding prevention, sub-keywords |
| Change only part of an active setup | 부분설정 | Quick edits without rebuilding all settings |

Core settings to explain:

- 입찰주기: rank check and bid execution interval in minutes.
- 입찰대상: device, region, exposure location, or gender/age depending on the Naver ad product.
- 희망순위: target exposure rank.
- 입찰기본가: fallback/reference bid used when rank cannot be checked and the base bid is higher than the current bid. It cannot exceed max bid.
- 최대입찰가: upper CPC limit for budget control.
- 입찰가감액: required adjustment unit for downward bidding. Use 0 KRW when unused.
- 하향입찰: when the target rank is maintained for configured checks, DIAD gradually lowers bids until just before dropping below the desired rank to help preserve rank with lower cost.

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

## Proposal Workflow

When building an ad proposal, structure the thinking in this order:

1. Client diagnosis
2. Request interpretation
3. Main performance strategy
4. Supporting media tests
5. Tracking/reporting plan
6. Risks and confirmation items
7. Client-facing proposal wording

For important RFP/proposal work, prefer this deck/story order:

1. Problem definition
2. Improvement strategy
3. Market/search environment
4. GabiaCNS capability and references
5. Support benefits and next steps

## Reference Loading Guide

Load only the references needed for the task:

- For WSEKR or education lead-generation proposals: read `references/wsekr-proposal.md`.
- For Naver Powerlink, ADVoost, expanded search, quality index, or auto-bidding: read `references/naver-search-advoost.md`.
- For Kakao, Naver GFA, Communication Ads, Power Content, and blog/cafe/media expansion: read `references/kakao-gfa-content.md`.
- For blog SEO/AEO and content writing rules: read `references/blog-seo-aeo.md`.
- For PPT proposal production and visual quality rules: read `references/ppt-proposal-guidelines.md`.

## WSEKR Default Positioning

For Wall Street English Korea-style RFPs, the strongest frame is:

> WSEKR's Naver performance decline is unlikely to be solved only by adding keywords or adjusting bids. GabiaCNS should position the proposal around search-intent-based account structure, ADVoost expansion control, landing and creative optimization using Naver optimization indicators, Daiad Pro rank-efficiency testing, and lead-quality feedback through CRM/BI data.

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

## Avoid

- "Run every possible channel" without budget and KPI logic.
- "PMax and Demand Gen will optimize" when the Google budget is too small or tracking is missing.
- "Lead generation campaign" without saying whether the lead comes from landing page form, Meta Instant Form, Google lead form asset, phone call, or Kakao route.
- "Manual targeting" without giving actual Meta and Google audience examples.
- "Kakao Brand Message" as if it can cold-target arbitrary Kakao users without channel friends, marketing opt-in users, or eligible consent data.
- "DIAD will guarantee conversions" or similar overclaims; DIAD is a bid/rank/CPC operation tool.
- "A/B testing" as only creative-copy testing for WSEKR; this is too narrow for the RFP and the performance problem.
- "ROAS improvement" without explaining CPL, CPA, consultation connection, qualified lead, contract, or revenue feedback.
