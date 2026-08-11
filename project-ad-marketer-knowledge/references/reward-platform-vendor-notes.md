# Reward platform vendor notes: Buzzvil and NBT Adison

Use this reference when responding to future reward ad, offerwall, app performance, affiliate/mission, or app partnership inquiries using the uploaded materials:

- NBT Adison platform/partnership introduction, 2026 Q2 upload.
- Buzzvil ad product introduction, ver. 2026-01-23 upload.

Treat these notes as vendor-material-derived guidance, not as current guaranteed terms. Always recheck the latest media sheet, unit price, eligible industries, targeting availability, tracking requirement, and reconciliation/deduction policy before proposing to a client.

## First distinction

Do not treat Buzzvil and NBT Adison as the same kind of source material.

- Buzzvil material is closer to an advertiser-facing media product introduction. It includes product types, billing concepts, targeting, examples, dashboard/reporting, and some unit-price references.
- NBT Adison material is closer to an offerwall/platform partnership introduction. It explains how a publisher/partner service can introduce an offerwall, API/SDK integration, placement/native exposure, mediation, admin, CS, and reward operation.

Client-facing implication:

- Use Buzzvil more directly when discussing reward media execution options for advertisers.
- Use NBT Adison mainly to explain how offerwall infrastructure, partner integration, reward program operation, and user engagement mechanics work.
- Do not quote NBT Adison as if it is a simple media-buying rate card unless a separate advertiser product sheet is confirmed.

## Buzzvil: practical ad product map

Buzzvil frames reward ads as a funnel product set from awareness to conversion.

| Funnel | Product type | Billing/product terms shown in material | Practical use |
|---|---|---|---|
| Awareness | Exposure/click reward ads | CPM, CPM+, CPC | Short-term traffic and brand/pro promotion reach. Click or landing-stay missions can generate large visits but may not imply lead quality. |
| Consideration | Quiz ads | CPQ, CPQ Lite | Brand/product/campaign-name recognition through quiz participation. Useful for launches and awareness, not direct lead quality. |
| Prospect pool | SNS mission ads | CPF, CPK, CPY, CPYLike, CPYView, CPNstore, CPL, CPTiktok | Follower, friend-add, subscription, store-alert, watch, like, or social engagement missions. Useful for owned-channel growth and CRM pool expansion. |
| Event traffic | Live commerce ads | Separate live-commerce pricing | Short-time traffic concentration during live broadcasts. Not relevant unless the advertiser has time-bound live content. |
| App growth | App inflow | CPI, CPE | App install or app open missions. Requires app linkage; MMP tracking link/function may have limitations depending on product. |
| App/commerce growth | UA specialized ads | UA, negotiated | Multi-mission structure where the final configured mission is billed. Best for app/game/commerce where onboarding or first-purchase funnel matters. |
| Retargeting | Retargeting ads | RCPM | Requires app ownership and all-postback linkage. Uses behavior/participation signals; should not be proposed without data-link readiness. |
| Conversion | Action ads | CPA | Higher-depth missions such as survey, signup, financial action, account opening, or consultation-type action. Requires web/app third-party integration and advance setup. |

## Buzzvil: unit-price caution

The uploaded Buzzvil material includes example/pricing references such as:

- CPC around 40 KRW per click in some products.
- CPQ/CPQ Lite minimum/package examples.
- SNS mission product examples for Instagram, Kakao channel, YouTube, Facebook, TikTok, and Naver Smart Store alerts.
- CPI/CPE examples.
- CPA examples by action depth, with many items requiring negotiation.
- Targeting surcharges and KakaoM-specific pricing can differ.

Do not paste these into a proposal as guaranteed current rates. Use:

```text
The uploaded Buzzvil 2026 product sheet includes reference pricing by product type, but final unit price, minimum budget, promotion rate, KakaoM applicability, targeting surcharge, and industry eligibility must be reconfirmed before quotation.
```

## Buzzvil: tracking and setup requirements

Important operational conditions from the material:

- UA, CPE, and CPA require platform/app connection before campaign launch; the material says linkage should be completed 7 days before launch.
- CPA requires web/app third-party integration.
- RCPM requires app ownership and all-postback linkage.
- MMP linkage with major third-party trackers is positioned as available.
- Dashboard reporting includes detailed indicators such as clicks and conversions for applicable products.

Proposal caution:

- If the advertiser does not have app tracking, MMP, SDK/S2S, or web conversion integration ready, avoid promising CPA/CPE/RCPM execution depth.
- If the advertiser's actual KPI is valid lead, consultation connection, opening, or contract, confirm whether Buzzvil accepts that deeper event as a billable/postback event. Otherwise report it internally as quality assessment rather than billing.
- If the platform does not provide a deduction guide, do not promise invalid-lead deduction.

## Buzzvil: targeting notes

The material lists broad/general and detailed targeting options such as:

- gender and age,
- region by city/province/district,
- device model,
- OS,
- carrier,
- ADID/GAID/IDFA based advertiser data targeting,
- prior campaign participation/retargeting,
- lifestyle/app-category based targeting,
- weather/fine-dust-related targeting,
- industry-specialized targeting.

Critical notes:

- ADID/GAID/IDFA targeting is app/device-identifier based and should not be assumed available for pure web campaigns.
- Under-14 or child-directed restrictions must be checked. The material notes Google family policy related restrictions for users under 14/under 13.
- Gender targeting may not be perfectly exclusive on some female-oriented media, according to the material's caveat.
- General targeting can incur surcharges, and detailed targeting may be limited by product type.
- Always confirm exact targeting availability by product, media inventory, OS, and privacy status.

## Buzzvil: when it fits

Stronger fit:

- app install/open campaigns,
- short-term traffic or awareness boost,
- social channel growth,
- quiz-based launch awareness,
- app/commerce onboarding,
- retargeting when app and postback data exist,
- financial/game/insurance or action-heavy campaigns where mission completion can be verified.

Weaker or caution fit:

- lead-generation advertisers that care about valid DB quality but cannot send valid/rejected status back,
- web-only advertisers with no click-ID/S2S/event integration,
- advertisers expecting bad DB deduction without a deduction guide,
- long-consideration services where rewarded action volume may not equal true intent.

## NBT Adison: platform and partnership notes

NBT Adison positions itself as an offerwall platform with partner-service integration and reward-program operation.

Useful concepts:

- API integration can support web offerwall surfaces.
- API + SDK integration can support partner UI/UX and app/web flows.
- JavaScript/WebView and SDK patterns can support service-specific ad experiences.
- Mediation can aggregate domestic and overseas ad networks and manage duplicate/priority/ad-quality logic.
- Placement, native ad, and deep link functions can expose offerwall ads in partner service surfaces rather than only in a standalone wall.
- Partner/admin functions can support in-house campaign registration, on/off status, ad/revenue reports, download, and data analysis.
- Partner-side exclusion controls can restrict competitor, same-category, specific product, price/amount, or other agreed ad types.
- CS and privacy consent handling are emphasized, including per-ad consent and additional personal-information submission pages where needed.
- Partner onboarding can require SDK integration, development, QA, marketplace review, and 4-6 weeks for standard SDK integration; more complex API/web integrations can take longer.

Proposal caution:

- Adison is especially useful for explaining publisher-side offerwall economics, user engagement, reward circulation, and partner-service integration.
- For advertiser media buying, request the separate advertiser product/rate card if needed.
- Do not promise expected revenue from generic MAU/DAU alone. Adison material itself says expected revenue depends on service, reward attractiveness, usable reward utility, traffic, demographics, and profiling.

## Client-facing explanation of reward media

Use this concise explanation:

```text
Reward media can create a clear action trigger because the user receives a benefit for completing a mission. This makes it strong for traffic, install, follow, quiz, and certain app/action events. However, for lead-generation campaigns, raw action volume and true business value can diverge. Therefore, reward media should be tested with a clear event definition, tracking readiness, valid-lead criteria, and post-campaign quality review.
```

## Recommended pre-check questions

For any future app/reward ad inquiry, ask:

1. Is the campaign app, web, or both?
2. Is the KPI traffic, install, app open, signup, social follow, quiz, inquiry submitted, valid lead, purchase, or contract?
3. Does the advertiser have MMP, SDK, S2S, or web third-party tracking ready?
4. Can the advertiser capture click ID, ADID/GAID/IDFA where applicable, lead ID, phone/email hash, or CRM ID?
5. Can raw conversion and validated conversion be separated?
6. Does the media accept qualified-lead postback, or only raw completion?
7. Is there a deduction/reconciliation guide for invalid leads?
8. Are target age, industry, and product allowed for the selected media/product?
9. Is the launch schedule compatible with required linkage/QA time?
10. Are unit prices and promotions current for the quarter?

## Proposal stance

Best stance:

```text
Reward media should be proposed as a volume-driving and event-verification channel, but scaling should be based on quality-adjusted performance: valid rate, connected consultation rate, downstream purchase/contract rate, and CRM status, not only raw CPA.
```

Avoid:

- saying reward CPA means guaranteed high-quality lead,
- mixing NBT partner-platform claims with Buzzvil advertiser-media products,
- quoting old rate-card numbers without reconfirmation,
- proposing RCPM/UA/CPA without MMP/postback/integration readiness,
- treating ADID targeting as available for web-only campaigns,
- promising invalid-lead deduction when no deduction guide exists.

## 2026-08-10 변경 요약: 애디슨 상담 신청 CPA 검증 조건

### 1) 새로 학습한 사실

- **사용자 제공 운영 조건:** 애디슨 광고주 집행 최소 예산은 500만원으로 전달됐다. 공개 고정 정책으로 확정하지 않고 집행 시점 매체 제안서 또는 담당자 확인이 필요하다.
- **제공 자료 기반 사실:** 애디슨 연동 구조는 참여 식별값과 완료 포스트백을 사용할 수 있다. UTM은 유입 캠페인 구분에는 유용하지만 보상 미션 완료와 과금 확인을 대신하지 않는다.
- **운영 판단:** 상담 신청 완료가 과금 이벤트라면 매체의 원문의와 내부 유효 문의를 분리해야 한다. 중복·허위·연락 불가·서비스 불가 문의가 자동으로 차감된다고 가정하지 않는다.

### 2) 기존 지식에서 수정할 점

- 최소 집행액이 큰 오퍼월을 소액 미디어믹스에 비율만 맞춰 넣지 않는다. 500만원은 월 600만원의 83.3%, 1,200만원의 41.7%, 2,000만원의 25%다.
- CPA 완료를 UTM만으로 확인한다고 설명하지 않는다. 참여 식별값, 완료 포스트백, 서버 간 전환 연동과 정산 규격이 별도로 필요하다.
- 원문의 CPA가 낮다는 이유만으로 성과가 좋다고 판단하지 않는다. 유효 문의율, 통화 연결률, 견적 발송률과 계약 진행률을 함께 비교한다.

### 3) 실무 적용 원칙

1. 월 600만원·1,200만원 규모에서는 먼저 일반 디스플레이·디멘드젠 등에서 유효 상담 기준을 만든다.
2. 애디슨 500만원을 전체의 25% 수준으로 편성할 수 있는 월 2,000만원 이상에서 1회 검증안으로 우선 검토한다.
3. 집행 전 업종 승인, 제휴 지면, CPA 단가, 참여 식별값, 완료 포스트백, 무효 문의 차감과 정산 기준을 서면으로 확정한다.
4. 서버 간 전환 연동을 구현할 개발 또는 유지보수 담당자가 없으면 집행을 보류한다.
5. 첫 검증 후 전체 문의 CPA와 유효 문의 CPA를 모두 보고 재집행 여부를 판단한다.

### 4) 제안서/리포트 문장 예시

> 애디슨은 최소 집행액 500만원을 상시 예산으로 편성하기보다 상담 신청 CPA의 1회 검증 예산으로 운영합니다. 매체 과금은 상담 신청 완료 기준으로 확인하고, 내부 성과는 중복·허위·연락 불가 문의를 제외한 유효 문의 CPA와 통화 연결률·견적 발송률로 평가합니다.

### 5) 다음 확인 필요사항

- 500만원 최소 집행액의 현재 적용 여부와 VAT·수수료 포함 범위
- 장기렌트·리스 업종 승인과 제휴 지면
- 무효 문의 차감·환급·정산 기준
- 참여 식별값과 완료 포스트백의 정확한 개발 규격
- 유효 문의 상태를 매체로 회신할 수 있는지와 과금 조정 가능 여부
