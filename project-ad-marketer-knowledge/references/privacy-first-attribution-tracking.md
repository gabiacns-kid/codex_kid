# Privacy-first attribution and server-side tracking

Use this reference when explaining cookie loss, MMPs, SDKs, S2S tracking, Meta CAPI, Google enhanced conversions, server-side GTM, SKAN/AdAttributionKit, or privacy-first conversion measurement in Korean ad proposals.

## 2026-09-03 변경 요약: 공개 태그 점검과 SA 식별 규격

### 1) 새로 학습한 사실

- 공개 HTML에서 GA4·Google Ads·Naver WCS·Kakao JavaScript SDK 같은 코드가 보이더라도, 설치된 태그와 실제 전환 이벤트가 정상 발화한다는 사실은 별도다. GTM이 동적으로 불러오는 태그는 공개 소스만으로 누락될 수 있다.
- Kakao JavaScript SDK 로딩은 Kakao Moment Pixel 설치를 뜻하지 않는다. SDK의 로그인·공유 기능과 광고 전환용 Pixel & SDK를 분리해서 확인한다.
- 검색광고 분석에서는 자동 클릭 식별자와 UTM의 역할을 나눈다. Google Ads 자동 태깅의 `gclid`는 Google Ads와 GA4 귀속에 우선 활용하고, 수동 UTM은 내부 캠페인·그룹·소재·키워드 비교 규격으로 사용한다.
- 문서 표기 제목을 `UTM_SOURCE`처럼 대문자로 쓸 수는 있지만 실제 URL 파라미터 키는 GA4 규격에 맞춰 `utm_source`, `utm_medium`, `utm_campaign`, `utm_term`, `utm_content`처럼 소문자로 유지한다. 값도 대소문자 차이로 행이 분리되지 않도록 규칙을 통일한다.

### 2) 기존 지식에서 수정할 점

- 페이지 소스에 태그 ID가 보인다는 이유로 구매·장바구니·회원가입 이벤트까지 정상 설치됐다고 확정하지 않는다.
- `Kakao SDK 확인`을 `Kakao Pixel 확인`으로 바꿔 쓰지 않는다.
- 네이버·구글 SA의 모든 키워드에 서로 다른 수동 URL을 직접 입력하는 작업만 제안하지 않는다. 플랫폼 추적 템플릿·동적 파라미터·자동 태깅 지원 범위를 먼저 확인한다.

### 3) 실무 적용 원칙

1. 1차 공개 점검: HTML·네트워크 요청에서 태그 컨테이너와 매체 ID 존재 여부를 확인한다.
2. 2차 브라우저 점검: GTM Preview/Tag Assistant, GA4 DebugView, 각 매체 픽셀 도구로 페이지뷰와 이벤트 발화를 확인한다.
3. 3차 거래 점검: 상품조회 → 장바구니 → 로그인·회원가입 → 결제 시작 → 테스트 구매 순서로 이벤트명, 값, 통화, 상품 ID, 주문번호를 확인한다.
4. 4차 중복 점검: 브라우저 태그와 서버 이벤트가 함께 발송될 때 `event_id`, `order_id`, `lead_id`로 중복 제거되는지 확인한다.
5. SA URL은 매체·캠페인·그룹·소재·키워드 구분을 공통 규격으로 설계하되, Google은 `gclid`를 삭제하거나 수동 UTM으로 대체하지 않는다.

### 4) 제안서/리포트 문장 예시

> 공개 소스에서는 일부 분석·광고 태그의 존재 여부만 확인할 수 있습니다. 실제 운영 전에는 태그 미리보기와 디버그 화면에서 상품조회, 장바구니, 결제 시작, 구매 이벤트가 정상 발화하는지 확인하고, 주문번호·매출값·통화·상품 ID와 중복 전송 여부까지 테스트하겠습니다.

### 5) 다음 확인 필요사항

- GTM 컨테이너 접근 권한과 게시 버전
- GA4 향상된 측정·전자상거래 이벤트 및 Google Ads 전환 액션 설정
- Naver WCS 구매값·주문번호 전송과 Kakao Pixel & SDK 이벤트 연동 여부
- Meta Pixel·Conversions API 설치 및 `event_id` 중복 제거 여부
- 모비온·타게팅게이츠 등 DSP의 전용 스크립트, 피드, 이벤트 규격과 매체 간 중복 귀속 기준

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
