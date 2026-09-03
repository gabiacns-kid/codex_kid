# Programmatic Advertising, DSP, SSP, DMP, RTB Reference

Use this reference when explaining programmatic advertising, DSP, SSP, DMP, ad exchange, RTB, or media-buying supply chains in Korean ad proposals, client education materials, blog posts, and internal strategy notes.

Primary checked source:

- Amazon Ads guide, "SSP와 DSP 의 차이점은 무엇인가요?", checked 2026-06-26.

## Core Definitions

DSP and SSP should not be explained as two similar ad platforms. They sit on opposite sides of the ad transaction.

- DSP (Demand-Side Platform): software used by advertisers, brands, and agencies to buy digital ad inventory programmatically across multiple media sources.
- SSP (Supply-Side Platform): software used by publishers and media owners to sell available ad impressions programmatically to many buyers.
- DMP (Data Management Platform): a data platform that stores and activates audience insights or audience segments for ad targeting.
- RTB (Real-Time Bidding): an auction-based programmatic buying method where each available impression can be bid on in real time.

Simple client-facing framing:

```text
DSP is the buying tool for advertisers.
SSP is the selling tool for media owners.
DMP is the audience-data tool that helps decide whom to target.
RTB is the real-time auction method used to buy and sell each ad opportunity.
```
## Easy Analogy

Use a market analogy when explaining this to non-marketers:

- Advertiser = the person who wants to buy a stall or display space to promote a product.
- Publisher/media owner = the person who owns the stall space.
- DSP = the buyer's purchasing agent. It compares many available spaces and decides where to buy within the advertiser's budget.
- SSP = the seller's sales agent. It exposes the seller's available spaces to many buyers and tries to sell them at the best price.
- Ad exchange = the marketplace where buyers and sellers meet.
- DMP = the customer-insight notebook used to decide which crowd or audience group is worth reaching.
- RTB = the instant auction that happens whenever one ad space becomes available.

## How DSP And SSP Work Together

1. A user opens a website, app, video, or other digital media surface.
2. The publisher has an available ad impression.
3. The SSP sends that impression opportunity to ad exchanges, DSPs, or ad networks.
4. The DSP checks whether the impression matches the advertiser's targeting, budget, frequency, bid, and campaign goal.
5. Buyers bid in real time when the impression is valuable to them.
6. The winning ad is shown to the user.
7. Performance data flows back to the buying platform and reporting systems.

## Proposal-Level Explanation

Use this wording when a client asks what DSP/SSP means:

```text
DSP는 광고주가 여러 매체의 광고 지면을 한 번에 비교하고 구매할 수 있도록 도와주는 구매 플랫폼입니다.
반대로 SSP는 언론사, 앱, 웹사이트 같은 매체사가 보유한 광고 지면을 여러 광고주에게 판매하고 수익을 높이기 위해 사용하는 판매 플랫폼입니다.
쉽게 말하면 DSP는 광고주 쪽의 구매 도구, SSP는 매체사 쪽의 판매 도구입니다.
두 플랫폼은 광고거래소와 실시간 입찰 구조를 통해 연결되며, 이 구조를 통해 광고주는 원하는 타겟에게 더 효율적으로 도달하고 매체사는 보유 지면의 판매 기회를 넓힐 수 있습니다.
```

## Practical Advertising Meaning

For agency strategy, DSP is more relevant to advertisers than SSP.

- Advertisers care about DSP because it affects audience targeting, inventory access, frequency control, budget allocation, and performance reporting.
- Publishers care about SSP because it affects fill rate, yield, floor price, buyer access, and inventory monetization.
- Agencies usually propose or operate DSP-side buying unless the client is a publisher or app/media owner.

## What Not To Overclaim

Avoid these misleading explanations:

- Do not say DSP itself guarantees conversions. It is a buying and optimization platform, not a guaranteed performance engine.
- Do not say SSP is something ordinary advertisers directly operate. SSP is mainly for media owners and publishers.
- Do not describe DMP as a database of exact customer identities. DMP data is usually audience/segment-oriented and often anonymous or pseudonymous.
- Do not imply every display ad buy uses open RTB only. Programmatic buying can include open auctions, private marketplaces, programmatic guaranteed, direct integrations, or platform-specific inventory.

## When To Mention DSP In Client Strategy

Mention DSP when:

- the advertiser needs broader reach beyond one closed media platform;
- the goal is awareness, reach, video/display exposure, or audience expansion;
- audience segmentation and frequency control matter;
- premium inventory, brand safety, or cross-media reach is important;
- the budget is large enough to learn across placements and audiences;
- measurement and conversion tracking are ready enough to judge results.

Be cautious when:

- budget is too small;
- there is no tracking or conversion path;
- the advertiser expects immediate lead or purchase performance from broad display exposure;
- creative assets are weak;
- the client actually needs search-intent capture first.

## Relationship To DMP And CDP

Use the DMP/CDP reference when explaining data-platform differences in more detail.

- DMP helps build or activate broader audience segments for paid media.
- CDP is better framed as known-customer profile and CRM activation infrastructure.
- DSP can use audience data from DMP, advertiser first-party data, platform data, or publisher signals depending on platform capabilities and consent conditions.

## Client-Friendly One-Line Summary

```text
DSP는 광고주가 광고 지면을 사는 도구, SSP는 매체사가 광고 지면을 파는 도구이며, 이 둘이 실시간 입찰과 데이터 기반 타겟팅으로 연결되면서 프로그래매틱 광고가 작동합니다.
```
