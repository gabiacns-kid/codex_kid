# Rewarded App and Offerwall Performance Ads

Use this reference when reviewing app reward ads, offerwall, CPA, CPQ, CPI, CPE, CPL, or mobile performance campaigns where the advertiser wants a downstream action such as lead submission, valid lead, consultation connection, purchase, contract, or activation.

## Core Principle

Separate **what the media can bill on** from **what the advertiser ultimately values**.

Rewarded media can often drive high action volume, but the lower the KPI goes in the funnel, the more it depends on advertiser-side tracking, CRM validation, and postback/reconciliation.

For lead-generation advertisers, always check the advertiser's tracking and CRM readiness before proposing offerwall or reward ads as a serious performance channel.

## Key Concepts

### MMP

An MMP, or Mobile Measurement Partner, is a neutral third-party measurement layer for app marketing. It measures which media source drove an install or in-app event and helps avoid duplicated self-attribution across Meta, Google, Kakao, reward media, and other channels.

Use this concept with clients as: MMP is the neutral referee that identifies which channel actually contributed to app installs and in-app conversions when multiple ad channels are running at the same time.

Common examples in Korea include AppsFlyer, Airbridge, Adjust, Branch, and Adbrix.

### Postback

A postback is the server-side signal sent from an MMP or tracking system to a media source to say that a user completed an action.

Typical flow:

1. User clicks a media ad.
2. User installs the app or completes an event.
3. The MMP detects the attributed event.
4. The MMP sends a postback to the media partner.
5. The media partner uses the postback for billing, reward payment, and optimization.

Use this concept with clients as: postback is the signal that tells the media partner, "this user actually converted."

### CRM

CRM is not just data storage. It is the customer relationship management cycle: collect customer data, segment users, take action such as calls, SMS, Kakao messages, emails, or push notifications, and measure the result.

MMP and CRM usually play different roles:

| Tool | Main role | Typical question answered |
|---|---|---|
| MMP | Attribution and app event measurement | Which ad/media drove this install or inquiry? |
| CRM or internal customer system | Customer status, communication, and lead quality | Is this lead valid, reachable, connected, opened, or contracted? |

For lead-gen performance ads, CRM does not have to be a commercial SaaS such as Salesforce, HubSpot, Braze, or Notifly. A proprietary admin, call-center system, inquiry database, or back-office table can play the same role if it records lead status and can export or transmit the status.

### S2S

S2S, or Server-to-Server, is a tracking method where the advertiser's server sends event data directly to an MMP or media partner instead of relying only on a browser pixel or app SDK.

SDK flow:

```text
User action -> app SDK detects event -> MMP receives event
```

S2S flow:

```text
User action -> advertiser server confirms event -> advertiser server sends event to MMP/media
```

Use S2S when:

- The event should be confirmed only after backend DB save.
- The advertiser wants to send CRM-qualified events such as valid lead, consultation connected, opening, contract, or purchase.
- Browser or SDK-only tracking may be incomplete.
- Sensitive data should be handled server-side.

S2S requires development resources, API/token management, event naming, user or click identifiers, and deduplication logic.

## Practical KPI Layers

1. Click or landing arrival
   - Usually trackable by the media click ID, UTM, or landing logs.
   - Too shallow for lead-generation businesses.
2. App install or first open
   - Trackable through MMPs such as AppsFlyer, Adjust, Airbridge, Branch, Adbrix, or Firebase/Google Ads app conversion setup.
   - Not sufficient if the business KPI is a valid inquiry.
3. App or web event completion
   - Trackable if the advertiser implements SDK, web pixel, server-side event, or S2S postback.
   - Example event: quote inquiry submitted.
4. Valid lead
   - Requires advertiser-side rules such as phone verification, required fields completed, duplicate removal, invalid phone removal, and serviceable-region check.
   - Media cannot reliably know this unless the advertiser sends validated conversion status back.
5. Consultation connected, activation, opening, contract, or revenue
   - Usually CRM/backend territory.
   - Can be reported or optimized only if the advertiser returns status updates through MMP/S2S postback, offline import, or a mutually agreed reconciliation file.

## Two-Step Lead Event Design

For inquiry-based reward ads, split events into at least two layers:

| Layer | Event example | Meaning | Main use |
|---|---|---|---|
| Step 1 | `lead_submitted` | Inquiry form was submitted or saved | Raw CPA, volume check, media delivery check |
| Step 2 | `lead_qualified` | CRM/internal DB confirmed it as valid | True performance evaluation and optimization |
| Step 2 negative | `lead_rejected` | Duplicate, fake, unreachable, or unserviceable lead | Exclusion, deduction, and quality feedback |

Do not optimize only to `lead_submitted` when the advertiser's actual KPI is valid lead, consultation connected, opening, contract, or revenue.

Ideal flow:

```text
Ad click
-> inquiry submitted
-> CRM/internal DB validates lead
-> advertiser sends S2S postback to MMP
-> MMP sends partner postback to media
-> media optimizes or reconciles against valid leads
```

Important caution:

- CRM validation can be delayed. The more delayed the postback, the weaker real-time media optimization becomes.
- The invalid-lead rule must be defined before launch.
- If the media cannot accept late qualified-lead postbacks, use post-campaign reconciliation or internal quality reporting instead of pretending the media can optimize to valid lead.

## What Is Usually Hard To Promise

- Exact final pricing method: media products have their own billing units and minimum payout/bid rules.
- CPQ meaning: not universally standardized. Confirm whether the vendor means Cost per Quest, quiz, quote, or another mission-type action.
- Guaranteed valid lead count before media benchmarks and validation rules are confirmed.
- Deduction of duplicates, fake leads, unreachable leads, or unserviceable leads unless exclusion criteria and evidence fields are pre-agreed.
- Optimization to consultation connected, installation completed, or contract if those statuses are not sent back from the advertiser system.
- User-level iOS attribution in all cases due to privacy and SKAN/ATT limitations.

## Advertiser Readiness Checklist

Before proposing app reward or offerwall media for a lead-generation advertiser, ask:

1. Is the primary path app, web, or both?
2. Is an MMP already installed? If yes, which one?
3. Are app events such as install, signup, and inquiry submitted already configured?
4. If web lead submission is used, can the advertiser send web events through an SDK, tag, or S2S API?
5. Is inquiry completion defined as button click, thank-you page, or backend DB save?
6. Is there a CRM, admin, call-center system, inquiry DB, or back-office table that manages lead status?
7. Can the advertiser identify duplicate, fake, unreachable, unserviceable, already-subscribed, or test leads?
8. Can lead status be exported or sent back through API/S2S/postback/offline file?
9. Is there an internal or external developer who can implement SDK, event mapping, S2S, click ID capture, and deduplication?
10. Is the privacy consent wording sufficient for inquiry, consultation, ad measurement, and data transfer where needed?

## Buzzvil and MMP Readiness

For Buzzvil specifically, start from the uploaded vendor-material baseline that linkage with major third-party trackers/MMPs is available. Do not describe Buzzvil-side MMP linkage as the main bottleneck unless the latest media confirmation contradicts this.

When a media partner such as Buzzvil says it can work with MMPs, interpret it carefully:

> This usually means the media can receive postbacks from major MMPs, not that the advertiser can skip MMP/tracking setup entirely.

For app install or in-app inquiry completion campaigns, assume that advertiser-side MMP setup is strongly recommended or practically required unless the media partner explicitly provides an alternative tracking method.

Possible exceptions:

- Simple click/landing campaigns.
- Web inquiry completion using media-provided tracking and advertiser S2S.
- A media partner's proprietary tracking link, SDK, or verification process.
- Offline reconciliation based on agreed lead files.

Client-facing confirmation question:

> If the advertiser is not currently using an MMP, can the media partner support inquiry-completion CPA through its own tracking or click-ID-based S2S postback? If the KPI is an in-app event, confirm whether MMP integration is mandatory. If the KPI is web inquiry completion, confirm whether S2S can replace MMP tracking.

## Recommended Response Frame

For lead-generation reward campaigns, recommend a staged test:

1. Define the primary billable action as inquiry submitted, but define valid lead separately.
2. Use phone verification, duplicate period, required fields, serviceable area, and unreachable criteria as the validation rule.
3. Confirm MMP, S2S, CRM/internal DB, and developer readiness before promising tracking depth.
4. Start with a small test budget across 2 to 3 media partners.
5. Compare raw inquiry CPA, valid inquiry CPA, valid rate, consultation connection rate, and downstream opening/contract status if available.
6. Scale only the media and offer messages that produce acceptable valid rate, not just low raw CPA.

## Client-Facing Caution

Do not say reward ads are unsuitable only because they are incentivized. Instead say:

> Reward ads can be useful for securing inquiry volume in a short period, but for lead-generation businesses where consultation feasibility and final activation matter, the campaign must be evaluated by valid inquiry rate and connected-consultation rate, not only by raw inquiry count. Start with a test, evaluate valid inquiry CPA by media source, and scale only the sources that meet the quality standard.
