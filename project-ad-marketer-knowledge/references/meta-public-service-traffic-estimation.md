# Meta public-service traffic estimation

Use this reference when estimating Meta results for public information platforms, education programs, youth services, or other awareness-plus-traffic campaigns from recent in-house reports.

## 1. New facts and evidence boundaries

- Meta's Traffic objective can optimize for link clicks, landing-page views, or daily unique reach. When a website visit is the stated goal and Pixel measurement is available, prefer landing-page-view optimization and cost per landing-page view as the main KPI.
- Advertisers can include people under 18 based only on age and location. Do not propose interest, behavior, gender, lookalike, or retargeting logic for the 13-17 segment as if it were available in the same way as for adults.
- Facebook and Instagram have a minimum user age of 13. Under-13 audiences require guardian-, teacher-, or institution-facing communication rather than direct Meta targeting.
- A source report labelled only as `click` does not prove that the metric is a link click or a completed landing-page view.

Official references checked 2026-07-21:

- https://www.facebook.com/business/ads/ad-objectives/traffic
- https://www.facebook.com/help/980264326141711/
- https://www.facebook.com/help/messenger-app/717368264947302/

## 2. What to correct in existing estimation habits

- Do not average row-level CTR, CPC, or CPM values. Sum spend, impressions, and clicks first, then recalculate weighted metrics.
- Do not mix search, commerce conversion, event engagement, or foreign-currency reports into a public-service traffic benchmark without a comparability explanation.
- Deduplicate files and campaign totals before aggregation. A renamed copy with different file metadata can still contain the same performance totals.
- Do not calculate expected results from the gross proposal amount when VAT and agency fees are included.
- Do not label estimated clicks as site visits when landing-page-view history is missing.

## 3. Practical application rules

When the gross budget includes 10% VAT and a 15% agency fee on net media spend:

1. supply amount = gross budget / 1.1
2. net media spend = supply amount / 1.15
3. net agency fee = supply amount - net media spend
4. media amount including VAT = net media spend × 1.1
5. agency fee including VAT = gross budget - media amount including VAT

For comparable campaigns:

- weighted CTR = total clicks / total impressions
- weighted CPM = total net media spend / total impressions × 1,000
- weighted CPC = total net media spend / total clicks
- expected impressions = planned net media spend / weighted CPM × 1,000
- expected clicks = planned net media spend / weighted CPC

Use case-level minimum and maximum values as a visible planning range. Do not manufacture an independent best-case combination from the lowest CPM, highest CTR, and lowest CPC when those values came from different campaigns.

If awareness and traffic are both requested but the budget and creative count are limited, consider one Traffic campaign optimized for landing-page views. Manage reach, impressions, and frequency as secondary awareness KPIs. Split Awareness and Traffic into separate campaigns only when reach or frequency is a contractual primary KPI and each campaign has enough budget and creative volume.

## 4. Proposal and report wording

Prefer:

- "최근 유사 목적의 실집행 사례를 가중 합산해 기준 예상치를 산정했습니다."
- "예상 클릭은 첨부 리포트의 클릭 정의를 따른 값이며, 실제 사이트 방문은 랜딩페이지 조회로 별도 확인합니다."
- "총예산에서 VAT와 대행수수료를 분리한 순수 매체비를 기준으로 성과를 환산했습니다."
- "13-17세는 연령·위치 중심의 넓은 도달로 운영하고, 18세 이상과 보호자 대상에서만 계정에서 허용되는 세부 타겟팅을 검토합니다."
- 인지도와 트래픽 목적을 함께 운영할 때는 전액 트래픽 기준 클릭 수를 통합 성과로 제시하지 않는다. 전액 트래픽 클릭 수는 비교치로만 표시하고, 실제 운영안의 클릭 참고치는 트래픽 캠페인 배정 예산에만 CPC를 적용한다. 인지도 캠페인에서 부수적으로 발생하는 클릭은 사전 예상치에 합산하지 않는다.

Avoid:

- "클릭 = 방문"
- "13-17세 관심사 타겟팅"
- "총예산 전액이 매체비"
- "패션 전환 캠페인의 CTR을 공공 플랫폼 트래픽 예상치로 그대로 적용"

## 5. Next checks before launch

- Confirm whether the Meta Pixel can record landing-page views on the final URL.
- Add UTM parameters and verify GA4 or the site's analytics tool.
- Confirm whether the report's `click` field means link clicks, all clicks, or another result metric.
- Check the live account's estimated audience size after separating 13-17 and 18+ groups.
- Recheck current teen-ad restrictions and optimization options in Ads Manager immediately before launch.
