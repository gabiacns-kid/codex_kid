# CDP and DMP Marketing Reference

Use this reference when explaining customer/audience data platforms in Korean advertising proposals, blog posts, media-mix plans, or client-facing strategy documents.

## Core Positioning

CDP and DMP are both data platforms, but they should not be described as the same tool.

- CDP (Customer Data Platform): a marketing and CRM-oriented platform for building and activating persistent customer profiles.
- DMP (Data Management Platform): an advertising and paid-media-oriented platform for creating anonymous audience segments and activating them in ad platforms.

Simple client-facing framing:

```text
CDP is for managing relationships with customers we know.
DMP is for targeting audiences we do not personally know.
```

Use an easy analogy:

- CDP = a regular-customer management book. It knows names, purchase history, preferences, and interaction history, so it can support personalized communication.
- DMP = a flyer distribution strategy. It does not know the person's real identity, but it can infer interest patterns and target similar audience groups with ads.

## CDP

CDP is generally used to collect, unify, store, and activate identifiable customer data.

Typical data:

- name, email, phone number, membership ID, hashed identifiers
- purchase history
- CRM and lead status
- website/app behavior connected to a known user
- offline/online customer interactions

Typical use cases:

- CRM segmentation
- remarketing to known customers
- personalized content or offer delivery
- lead nurturing
- lifecycle marketing
- connecting sales, service, and marketing records
- customer value analysis such as LTV, repeat purchase, churn risk

Proposal wording:

```text
CDP is useful when the advertiser wants to manage known customer data over the long term and connect marketing actions with CRM, sales, or service data.
```

## DMP

DMP is generally used to collect and classify anonymous audience data for advertising activation.

Typical data:

- cookie or device-based anonymous IDs
- browsing and content interest signals
- audience segments from partner data or external data providers
- broad attributes such as age range, interest, purchase intent, category affinity

Typical use cases:

- paid-media audience targeting
- programmatic advertising
- lookalike or similar-audience expansion
- prospecting campaigns
- audience segmentation by interest or intent
- campaign-level media buying support

Proposal wording:

```text
DMP is useful when the advertiser wants to find new potential customers at scale through anonymous audience segments and paid-media targeting.
```

## How DMP Collects Data

Explain DMP data collection in three levels:

1. First-party data
   - Data collected from the advertiser's own website/app.
   - Examples: page views, dwell time, product clicks, cart behavior.

2. Second-party data
   - Another company's first-party data used through a partnership or data-sharing relationship.
   - Example: a partner media company or commerce partner sharing consented segment data.

3. Third-party data
   - Aggregated audience data from external data providers or brokers.
   - Examples: broad segments such as "sports interest," "auto purchase intent," or "frequent traveler."

After collection, the DMP classifies people into audience segments such as:

- people who visited a certain product category multiple times,
- people interested in cars,
- people likely to travel,
- people similar to a high-value customer audience.

Those segments can then be activated in ad platforms or DSPs.

## CDP + DMP Together

The two can work together when a client has both CRM data and paid-media expansion needs.

Typical flow:

```text
DMP brings in or expands anonymous potential audiences.
CDP turns known customers/leads into long-term relationship and performance data.
```

Better proposal framing:

```text
DMP is used for audience discovery and paid-media expansion, while CDP is used after identification to connect the user to CRM, personalization, retention, and customer-value improvement.
```

## Critical Notes

- Do not overstate DMP precision. DMP audiences are usually segment-based and probabilistic, not the same as confirmed customer identity.
- Do not call a DMP a CRM tool. Its main role is advertising activation.
- Do not call a CDP only an ad-targeting tool. Its strength is persistent customer profile management and activation across marketing, sales, and service.
- Be careful with cookie-based wording. DMPs have historically relied heavily on cookies and third-party data, but privacy regulation, browser restrictions, and platform changes have reduced the reliability of traditional third-party cookie-based targeting.
- In proposal copy, use "anonymous or segment-based audience data" instead of saying only "cookie data."
- If a claim depends on current browser policy, privacy law, or platform-specific data use rules, verify current official documentation before finalizing.

## Proposal Decision Guide

Use CDP when:

- the advertiser has meaningful first-party customer data,
- CRM or membership data matters,
- repeat purchase, retention, lead nurturing, or personalization matters,
- performance should be judged beyond clicks and conversions, such as LTV or lead quality.

Use DMP when:

- the advertiser needs new prospect reach,
- anonymous audience targeting is enough,
- campaign goal is paid-media expansion,
- the advertiser wants to buy or activate interest/intent segments.

Use both when:

- the advertiser has first-party customer data and also wants to expand to similar potential audiences,
- CRM data can define high-value audiences and paid media can use those signals for prospecting or lookalike expansion.

## Sources To Check When Needed

- Adobe: CDP vs CRM vs DMP differences.
- Oracle: CDP and DMP difference; DMPs mainly pursue third-party data and short-term storage.
- Twilio Segment: CDP vs DMP; CDP for persistent customer data and DMP for anonymous advertising audiences.
- Salesforce or platform privacy resources when discussing first-party data and third-party cookie changes.
