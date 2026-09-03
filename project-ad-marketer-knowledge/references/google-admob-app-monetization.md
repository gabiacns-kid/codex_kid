# Google AdMob App Monetization

Use this reference when explaining Google AdMob, app monetization, in-app ad inventory, mediation, rewarded ads, app open ads, app-ads.txt, AdMob payments, invalid traffic, or when a client asks about app publisher revenue rather than ordinary Google Ads media buying.

Official sources checked:

- https://admob.google.com/home/
- https://support.google.com/admob/answer/6128738
- https://support.google.com/admob/answer/7356219
- https://support.google.com/admob/answer/2772208
- https://support.google.com/admob/answer/9787936
- https://support.google.com/admob/answer/9388275
- https://support.google.com/admob/answer/9691433
- https://developers.google.com/admob

Before client delivery, re-check current official AdMob Help and Google Developers pages for SDK version, ad format status, payment thresholds, policy wording, and country/currency conditions.

## Core Positioning

AdMob is not primarily an advertiser-side campaign product. It is a mobile app monetization platform for app developers and publishers.

Client-facing wording:

> Google AdMob은 앱 개발자와 퍼블리셔가 모바일 앱 안에 광고 지면을 만들고, Google 및 외부 광고 수요를 통해 앱 트래픽을 수익화할 수 있도록 지원하는 모바일 앱 수익화 플랫폼입니다. 일반 Google Ads처럼 광고주가 직접 매체를 구매하는 상품이라기보다, 앱 인벤토리의 수익화를 관리하는 퍼블리셔 도구로 이해해야 합니다.

Agency caution:

- For an advertiser proposal, do not present AdMob as a normal media-buying channel unless the buying route is clearly Google Ads app campaign/display/video inventory.
- For an app publisher/developer proposal, discuss AdMob as monetization, mediation, ad-format UX design, SDK integration, and policy-risk management.

## How AdMob Works

AdMob works by letting the developer create ad units and place those ad units in the app code. The ad unit sends ad requests to AdMob and displays matching ads.

Key IDs:

- **App ID**: identifies the app in AdMob.
- **Ad unit ID**: identifies each ad unit and is inserted into app code to request ads.

Implementation usually requires:

- Creating the app and ad units in AdMob.
- Adding Google Mobile Ads SDK to the app.
- Adding app ID and ad unit IDs to the app implementation.
- Testing with demo ads or test devices before production.
- Verifying app-ads.txt where required.

## Ad Formats

AdMob official Help lists these core ad formats:

- **Banner**: basic ad format at the top or bottom of the screen.
- **Interstitial**: full-page ads at natural breaks and transitions, such as level completion; supports video.
- **Rewarded interstitial**: full-page format that rewards users for viewing ads during natural breaks or transitions. Official Help marks this as beta in the checked page, so verify current status.
- **Rewarded**: rewards users for watching short videos or interacting with playable ads/surveys; useful for free-to-play or value-exchange experiences.
- **Native advanced**: customizable format that matches the app look and feel and appears inline with app content; supports video.
- **App open**: appears when users open or return to the app and overlays the loading screen.

Proposal caution:

- Choose ad formats by UX moment, not only revenue potential.
- Full-screen formats need natural breaks; poor placement can hurt retention and trigger accidental-click risk.
- Rewarded ads need a clear value exchange and abuse prevention.
- App open ads should be handled carefully around loading and returning sessions.

## Mediation, Bidding, and Waterfall

AdMob Mediation helps manage multiple ad sources and app revenue in one place.

Official AdMob positioning:

- AdMob Network can compete for app ad space.
- Mediation can use many networks globally.
- Bidding calls participating networks simultaneously so ad sources can bid on each impression in real time.
- Google describes bidding as helping earn the highest CPM for each impression.

Use this distinction:

- **Bidding**: participating ad sources compete in real time for the same impression.
- **Waterfall**: ad sources are called in a configured sequence, often based on expected eCPM.
- **Hybrid**: bidding and waterfall sources can be combined depending on available networks and SDK/adaptor readiness.

Agency caution:

- Do not promise bidding always outperforms waterfall. It depends on eligible partners, geography, app category, traffic volume, SDK setup, and demand.
- Mediation adds operational complexity: adapters, partner accounts, privacy requirements, test mode by network, and reporting reconciliation.

## app-ads.txt

app-ads.txt identifies authorized sellers of app ad inventory and helps prevent counterfeit app inventory.

Practical meaning:

- The file must be publicly available and crawlable.
- It gives advertisers and exchanges a way to know who is authorized to sell the app inventory.
- Google warns that failing to implement app-ads.txt can risk significant ad revenue loss.

Proposal caution:

- Do not describe app-ads.txt as optional hygiene only. For monetization, it can directly affect revenue protection.
- Check whether the developer website is correctly linked and crawlable.

## Payments and Thresholds

AdMob payment thresholds vary by reporting currency and should be checked in the official payment threshold table.

For USD accounts in the official threshold page checked:

- Tax information: USD 0.
- Verification: USD 10.
- Payment method selection: USD 10.
- Payment: USD 100.
- Cancellation: USD 10.

Client-facing caution:

- Do not state USD thresholds as universal. Thresholds differ by reporting currency.
- Estimated earnings and payment-history confirmed earnings can differ.
- Address/identity verification and payment holds can delay payment.

## Testing and Invalid Traffic

During development and QA:

- Use Google-provided demo ad units or test devices.
- Publishers must not click their own production ads, even for testing.
- Demo ad units are not associated with the publisher's AdMob account, reducing invalid-traffic risk.
- Test devices allow production-looking ads in test mode using the publisher's own ad unit IDs.
- In mediation, AdMob test mode applies to AdMob Network ads only; third-party ad sources need their own test-mode handling.

Client-facing caution:

> 개발 중 실제 광고 단위를 그대로 클릭해 테스트하면 무효 트래픽 정책 위반으로 이어질 수 있습니다. QA 단계에서는 데모 광고 단위 또는 테스트 기기를 설정하고, 미디에이션 사용 시 각 서드파티 네트워크의 테스트 설정까지 별도로 확인해야 합니다.

## Policy and Compliance Watchpoints

Key policy-sensitive areas:

- Invalid traffic, self-clicking, accidental-click inducement, automated traffic, or misleading UI.
- Children/families apps: Google Play Families policy, child-directed treatment tagging, maximum ad content rating, and self-certified ad SDK/mediation source requirements.
- Privacy and identifiers: especially Android/iOS advertising IDs, consent requirements, and platform policy changes.
- Content suitability and ad blocking controls.

For apps targeting children or mixed audiences:

- Ad requests may need child-directed treatment tags and max ad content rating settings.
- Mediation sources must also be compliant where Google Play Families policy applies.

## Strategic Proposal Frame

For an app publisher:

1. Diagnose the app category, DAU/MAU, session length, user flow, retention, and key UX breakpoints.
2. Map formats by user moment: banner for persistent light monetization, interstitial/app open for transitions, rewarded for value exchange, native for content feeds.
3. Add SDK/app ID/ad unit/app-ads.txt/testing readiness checklist.
4. Start with conservative placements, then optimize by ARPDAU, eCPM, fill rate, retention, and user complaints.
5. Use mediation/bidding only after baseline ad serving and reporting are stable.
6. Separate estimated revenue from actual payment eligibility and policy-compliant earnings.

For a marketer explaining AdMob:

- Emphasize that AdMob is publisher-side monetization.
- If the objective is to advertise to app users, explain the buying-side route separately through Google Ads and app/display/video inventory.

Strong wording:

> AdMob 운영의 핵심은 광고 형식을 많이 넣는 것이 아니라, 앱 사용 흐름 안에서 이탈을 만들지 않는 지점에 광고 단위를 설계하고, SDK·app-ads.txt·테스트 광고·정책 준수까지 안정적으로 갖춘 뒤 eCPM, 유효 노출률, 유지율, ARPDAU를 함께 보며 수익화를 고도화하는 것입니다.

## Common Mistakes to Avoid

- Calling AdMob a general advertiser-side ad product.
- Promising revenue from the AdMob calculator or sample figures.
- Treating app-ads.txt as minor setup.
- Testing with live production ads.
- Ignoring mediation partner test settings.
- Recommending interstitial/app open overuse without retention risk.
- Comparing rewarded, native, interstitial, and banner only by eCPM without UX context.
