# Privacy-first attribution and server-side tracking

Use this reference when explaining cookie loss, MMPs, SDKs, S2S tracking, Meta CAPI, Google enhanced conversions, server-side GTM, SKAN/AdAttributionKit, or privacy-first conversion measurement in Korean ad proposals.

## Core positioning

Do not frame the topic as "tracking is impossible now." The better proposal frame is:

> Browser, OS, and privacy-policy changes make shallow client-side tracking less reliable, so the advertiser needs a hybrid measurement structure that combines first-party data, SDK/pixel events, server-side events, MMP attribution, and CRM lead-quality feedback.

For lead-generation advertisers, always distinguish:

- raw conversion: inquiry submitted, signup, install, or form completion.
- validated conversion: valid lead, consultation connected, opened, contracted, or revenue confirmed.
- billable media event: the event the media partner accepts for billing.
- optimization event: the event the platform can actually learn from.

## Correct current facts

### Chrome third-party cookies

- Do not say Chrome has fully deprecated third-party cookies.
- As of Google's April 2025 Privacy Sandbox update, Chrome maintained the current approach of offering users third-party cookie choice and did not roll out a new standalone third-party-cookie prompt.
- The practical implication is still the same for proposals: third-party cookies are less dependable because of browser controls, consent, ad blockers, Safari/Firefox restrictions, Incognito restrictions, and platform privacy changes.

Client-facing wording:

```text
Chrome has not simply removed all third-party cookies, but user choice, browser controls, and privacy regulation have made third-party-cookie-based measurement less dependable. Therefore, first-party data and server-side measurement should be prepared as the more stable operating layer.
```

### Privacy Sandbox on Android

- Be careful: older materials may describe the Android Privacy Sandbox Attribution Reporting API as a future core attribution engine.
- Google announced in October 2025 that several Privacy Sandbox technologies, including Attribution Reporting API for Chrome and Android, Topics, Protected Audience, SDK Runtime, IP Protection, and others, are being retired.
- Therefore, do not propose Android Privacy Sandbox ARA as a current core architecture unless the exact API status is rechecked.

Client-facing wording:

```text
Privacy-preserving attribution APIs have been tested by major platforms, but API status changes quickly. For practical campaign design, the safer architecture is MMP/SDK + server-side event transmission + CRM validation rather than relying on a single browser or OS attribution API.
```

## MMP role

An MMP is the neutral measurement and attribution layer for app marketing.

Use MMP when:

- multiple media sources can claim the same install or app event,
- app install and in-app event measurement matters,
- deduplication and attribution rules need a neutral basis,
- media postbacks are needed,
- SKAN or AdAttributionKit reporting needs to be interpreted,
- app events must connect to downstream CRM or revenue signals.

Do not overstate MMP:

- An MMP does not automatically validate lead quality.
- An MMP does not replace CRM.
- An MMP does not solve all iOS attribution loss.
- An MMP can only optimize to valid leads if the advertiser sends valid-lead status back through events, postbacks, S2S, or offline imports and the media accepts those signals.

## SDK

SDK is the app-side measurement component.

Use SDK when:

- app install, first open, app event, deep link, or deferred deep link matters,
- app events need to be detected in the app,
- MMP attribution is needed,
- Apple Search Ads, SKAN/AdAttributionKit, or iOS app attribution needs to be interpreted.

S2S-only can be useful, but do not casually recommend replacing SDK entirely. SDK-only and S2S-only both have gaps.

## S2S tracking

S2S means the advertiser server sends event data to an MMP or media partner server.

Use S2S when:

- the event should be confirmed only after backend DB save,
- CRM/backend status such as valid lead, consultation connected, opening, contract, or revenue must be sent,
- browser pixels may miss events,
- data should be controlled and filtered server-side,
- offline or delayed conversions must be imported.

Critical limitations:

- S2S requires developer resources, API/token management, event naming, identifiers, and deduplication logic.
- S2S does not magically create attribution if the original click ID, app attribution ID, MMP attribution, or user identifier is missing.
- For web, click IDs, UTMs, first-party cookies, phone/email hash, lead ID, and backend save logs matter.
- For app, SDK/MMP identifiers, app event setup, and platform privacy rules matter.
- If media does not accept qualified-lead postbacks or deductions, S2S qualified events may be useful for internal reporting but not for billing adjustment.

## Hybrid tracking

Prefer a hybrid structure for serious performance proposals:

```text
Client-side signal: pixel, SDK, web tag, app event
+ Server-side signal: S2S, CAPI, enhanced conversions, offline import
+ First-party identity: email, phone, lead ID, CRM ID, hashed when required
+ Deduplication: event_id/order_id/lead_id shared across client and server
+ CRM validation: valid lead, connected consultation, contract, revenue
```

### Meta Conversions API

Meta CAPI creates a direct connection between advertiser marketing data from a server, website platform, app, or CRM and Meta systems.

Best proposal wording:

```text
Meta Pixel and Conversions API should be used together where possible. Pixel captures browser-side behavior, while CAPI sends more reliable server-side events such as lead submission, qualified lead, or offline conversion. When both send the same event, event identity must be matched to prevent duplicate counting.
```

Do not say CAPI bypasses privacy rules. Meta states CAPI is not a way to bypass iOS ATT, ePrivacy, or other data-sharing policies.

### Google enhanced conversions

Google enhanced conversions use first-party customer data such as email or phone, generally hashed with SHA-256, to improve conversion measurement and bidding.

Use in proposals when:

- lead or purchase forms collect first-party identifiers,
- Google Ads conversion accuracy is important,
- offline lead stages are imported,
- privacy-safe matching needs to be improved.

Do not imply it works without captured identifiers. If the lead form does not collect usable email/phone/name/address data, enhanced conversions cannot meaningfully match users.

### Server-side GTM

Server-side GTM acts as a first-party buffer between the user and vendors.

Useful benefits:

- stronger privacy and data control,
- improved data quality,
- reduced browser/vendor exposure,
- potential performance improvement by reducing client-side tag load.

Critical caution:

- Do not sell sGTM as a magic ad-block bypass or guaranteed conversion recovery tool.
- It needs server cost, implementation, consent handling, tag mapping, QA, and ongoing maintenance.

## SKAN and AdAttributionKit

Apple's privacy-preserving app attribution has evolved from SKAdNetwork naming toward AdAttributionKit.

Use conservative wording:

```text
iOS app attribution should be interpreted through MMP reporting, SKAN/AdAttributionKit signals, and platform-reported data together. It is not a user-level replacement for IDFA-based attribution.
```

Avoid:

- claiming full user-level attribution on iOS,
- treating SKAN as a complete substitute for MMP,
- assuming all downstream events can be measured with the same precision as Android/web.

## CMP vs MMP

MMP and CMP solve different problems.

| Tool | Role | Main question |
|---|---|---|
| MMP | Attribution and app performance measurement | Which media source drove the install or app event? |
| CMP | Consent and privacy governance | Did the user consent to the required data collection and transfer? |

Do not say MMP handles consent management unless the specific vendor provides consent-related integrations. CMP is the consent log and governance layer; MMP is the attribution and performance layer.

## Proposal checklist

Before recommending advanced tracking, confirm:

1. Is the conversion path app, web, or both?
2. Is there an MMP? Which one?
3. Are SDK and app events already installed?
4. Are pixels/tags already installed on web?
5. Can the advertiser capture click ID, UTM, lead ID, email/phone, or another matching key?
6. Can the advertiser send S2S events or offline conversion imports?
7. Is there CRM or backend lead-status data?
8. Are valid-lead/rejected-lead criteria pre-agreed?
9. Does the media partner accept qualified-lead postbacks or only raw submissions?
10. Is consent wording sufficient for measurement, advertising, and data transfer?

## Critical proposal stance

For lead-generation media such as reward ads or offerwalls, never promise:

- "valid lead CPA" if the media only bills on raw inquiry submission,
- "deduction of bad leads" if there is no deduction guide or reconciliation agreement,
- "full app attribution" without MMP/SDK/event setup,
- "server-side tracking will solve all missing conversions."

Better wording:

```text
The campaign can be launched on raw inquiry completion, but final performance should be judged by valid inquiry rate, connected-consultation rate, and downstream activation. If the media partner does not support deduction or qualified-lead postback, valid-lead data should be used as internal quality reporting and scale/stop criteria rather than as automatic billing adjustment.
```
