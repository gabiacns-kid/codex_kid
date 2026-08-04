# Naver Search, ADVoost, and Auto-Bidding Reference

## Powerlink Basics

Powerlink is keyword-based Naver search advertising. It is suitable for service and lead-generation advertisers when users actively search for a solution.

For education lead generation, do not judge success only by click or lead volume. Track:

- CTR
- CPC
- CVR
- CPL/CPA
- Consultation connection
- Reservation/visit
- Registration
- Revenue/ROAS if available

## Quality and Optimization Indicators

Naver search performance depends on relevance and expected click quality. Use indicators as operation triggers:

- Keyword and ad relevance
- Landing URL relevance
- Ad copy match
- Click expectation
- Conversion quality

If relevance is weak, review:

- Landing title/description and page content
- Mobile page quality
- Ad copy promise
- Keyword grouping
- Whether one URL is serving too many different intents

## ADVoost / Expanded Search

Treat ADVoost and expanded search as an operating environment, not an enemy.

Expanded search can expose ads to search terms not manually registered when the system judges the ad group, landing URL, and ad content relevant.

Operational rules:

1. Use expanded search to discover new intent.
2. Review search term reports regularly.
3. Classify terms into:
   - Promote to exact/controlled keyword
   - Observe
   - Add negative
   - Reflect in landing/content
4. Move high-value terms into controlled ad groups.
5. Match each intent to ad copy and landing.
6. Manage waste through negative keywords and grouping.

Proposal wording:

> 확장검색은 신규 검색어를 발견하는 탐색 장치로 활용하고, 검색어 리포트에서 성과 가능성이 확인된 검색어는 정식 키워드로 승격해 직접 관리하겠습니다. 승격 키워드는 별도 광고그룹 또는 기존 의도 그룹에 편입하여 입찰가, 소재, 랜딩 URL을 통제하고, 저효율 검색어는 제외 키워드로 관리해 확장성과 효율성을 동시에 확보하겠습니다.

## Match Type Logic

- Exact: registered keyword directly matches.
- Similar exact: close variant of registered keyword.
- Expanded: unregistered search terms can match based on ad/landing relevance.

Use exact/control for high-value terms; use expanded/search discovery with guardrails.

## Landing Readiness for AI-Based Matching

For Naver's AI expansion and relevance evaluation, landing pages should be crawlable and semantically clear.

Check:

- Page title clearly describes the page.
- Description summarizes the content.
- Main content is in text, not only image.
- Key benefits and course information are accessible in HTML.
- Mobile page is usable.
- No broken redirects, login walls, captcha, or blocked crawler.
- Each intent has the most relevant landing page.

## Daiad Pro / Auto-Bidding Differentiation

Use GabiaCNS's auto-bidding solution as a proposal differentiator.

Do not simply say "we maintain top rank." Stronger proposal:

- Segment keywords by role: main conversion, high CPC, brand defense, test/discovery.
- Test target positions by week or two-week periods.
- Compare CPC, CVR, CPA, ROAS by rank range.
- Find the most efficient position, not always #1.
- Use auto-bidding to maintain rank with minimum necessary bid.

Proposal wording:

> 가비아CNS는 단순 상위 노출이 아니라 키워드별 목표 순위와 수익성을 함께 검증합니다. 주요 전환 키워드, 고CPC 키워드, 고과금 키워드를 분류하고 주간 또는 격주 단위로 순위별 CPC·CVR·CPA·ROAS 변화를 비교해 가장 효율적인 노출 포지션을 찾겠습니다.

## Tracking Parameters

Naver search ads can use automatic tracking URL parameters and substitution variables.

Important parameters:

- `n_campaign_type`
- `n_ad_group`
- `n_media`
- `n_ad`
- `n_keyword`
- `n_keyword_id`
- `n_query`
- `n_match`
- `n_rank`
- `n_ad_group_type`

Important:

- `n_query` is the user's actual search query.
- `n_match` helps distinguish match type.
- Expanded search may not provide keyword id in the same way as registered keyword traffic.
- Always test landing URLs after adding parameters.

## 2026-07-10 Learning: ADVoost Max / Naver AI Briefing Ads

### 1. Source And Verification Status

- Official source checked on 2026-07-10: Naver Ads notice `네이버 AI 광고 출시 안내`, notice no. 31888, published 2026-06-15: https://ads.naver.com/notice/31888
- Additional source: user-provided Naver search ad operator notice pasted on 2026-07-10 describing ADVoost Max settings, insight report, disallowed industries, and reporting limits. Treat the pasted operator notice as user-provided current guidance unless the exact official notice URL is separately verified.

### 2. Officially Verified Facts From Notice 31888

- Naver AI ads start with `통합검색 > AI 브리핑`.
- Ad-center open date: 2026-07-15.
- Exposure open date: 2026-07-21.
- The official notice states the target product for formal service opening is `ADVoost 검색 광고`.
- AI Briefing ads appear only where Naver's ad agent judges ad exposure suitable.
- The ad is text-form and is intended to blend with AI Briefing content; format can change later.
- Ad copy is written by Naver's ad agent using advertiser-center and landing-page information; advertisers cannot directly edit that AI-written copy.
- AI ads can be controlled at ad-group registration/edit screens. At launch, ad groups using expanded search are set to ON by default.
- Targeting: time/day targeting is provided. Region, gender, age, and user segment targeting are used as hints for ad selection rather than deterministic selection controls.
- Billing is CPC. The CPC is based on the average Powerlink price related to the AI Briefing content, and a separate bid cannot be set.
- AI ads are exposed regardless of whether the advertiser registered the exact keyword. They use expanded-search budget, so the expanded-search budget cap must not be set too low if exposure is desired.
- Separate AI ad insight reporting is expected.
- Landing/advertiser readiness items:
  - schema.org fields such as `@type`, `name`, `description`, `price`, and `aggregateRating`;
  - readable site name in business channel information;
  - conversion script installation.
- The official notice says medical ad creatives subject to review may be restricted from AI Briefing exposure.
- AI ads can match all valid URLs in the ad group regardless of creative or keyword distinction.
- Final ad selection is handled by Naver's ad agent.

### 3. User-Provided Operator Guidance To Treat Carefully

The user's pasted operator guidance adds details that should be used with a source note until the exact official URL is confirmed:

- ADVoost Max is set in the existing expanded-search by ADVoost area at ad-group level.
- Ad groups using expanded search are ON by default at ad-center open; advertisers who do not want it should switch OFF.
- ADVoost Max performance appears in `검색광고 > 보고서 > ADVoost Max 인사이트`.
- Existing ad-management screens show only the total aggregate for ADVoost Max results.
- Targeting-level performance for region, gender, age, and user segments is not separately provided because those signals are only hints for ad selection.
- `내 광고 보기` can show where the AI agent exposed the ad and what AI-written ad text appeared, but not all AI-written texts are provided; it updates weekly on Monday when statistically meaningful.
- Pasted guidance lists disallowed industries as finance/insurance, health functional foods, and medical. This is broader than the official 31888 notice excerpt, which explicitly mentions medical-review restrictions. Verify before client delivery.
- Excluded keywords do not work for ADVoost Max because exposure is not directly matched to user search terms.
- ADVoost Max-specific performance is not separately provided in multidimensional/bulk reports beyond the ADVoost Max insight screen and aggregate totals in the basic ad-management screen.

### 4. Proposal And SEO/AEO Application

Use ADVoost Max as a conditional Naver expansion proposal when a Gmarket seller also appears to operate a self-owned mall or official site.

Positioning:

- ADVoost Max is not a classic manual keyword-rank product.
- It is closer to a context-matching AI search ad that uses AI Briefing context, ad-group/advertiser-center information, and landing-page content.
- Therefore, SEO/AEO readiness becomes part of paid-search readiness:
  - crawlable landing content,
  - schema.org product/local-business markup,
  - clear site name,
  - page title/description,
  - product/service description,
  - conversion script,
  - content that answers user exploration intent.

Client-facing wording:

```text
자사몰을 함께 운영 중이라면 G마켓 광고와 별도로 네이버 검색/AI 브리핑 영역까지 확장 검토가 가능합니다. ADVoost Max는 사용자가 직접 등록한 키워드에만 노출되는 구조가 아니라, 네이버 광고 에이전트가 AI 브리핑 문맥과 랜딩페이지 정보를 함께 판단해 광고를 선출하는 방식입니다. 따라서 단순 입찰가보다 사이트 이름, 랜딩페이지 설명, schema.org, 전환 스크립트 등 SEO/AEO 기반 점검이 중요합니다.
```

```text
다만 ADVoost Max는 별도 입찰가를 설정하는 상품이 아니며, 제외 검색어도 기존 검색광고처럼 작동하지 않습니다. 따라서 운영 전에는 자사몰의 랜딩 품질, 전환 추적, 업종 가능 여부, 확장검색 예산 비율을 먼저 점검한 뒤 테스트하는 것이 좋습니다.
```

### 5. Cautions Before Client Delivery

- Verify final ADVoost Max product name, eligibility, industry restrictions, report fields, and default ON behavior against current Naver official notices/help before formal proposal delivery.
- Do not propose ADVoost Max to restricted industries without confirmation. User-provided guidance says finance/insurance, health functional foods, and medical are unavailable; official notice 31888 explicitly mentions medical-review restrictions.
- Do not promise keyword-level control, negative-keyword exclusion, age/gender/location performance breakdown, or direct ad-copy editing.
- Because AI ad copy uses advertiser-center and landing-page information, poor site content can create weak or mismatched AI-generated messaging.

## 2026-07-30 update: ADVoost Max launch confirmation

### 1) 새로 학습한 사실

- Naver's official 2026-07-08 notice confirmed the ADVoost Max advertiser-center opening on 2026-07-15 and ad serving opening on 2026-07-21.
- ADVoost Max is controlled at ad-group level within the existing `확장검색 by ADVoost` setting. Ad groups already using expanded search were scheduled to default to ON at advertiser-center opening.
- AI Briefing performance is checked in `검색광고 > 보고서 > ADVoost Max 인사이트`. The basic ad-management screen shows aggregate ADVoost Max results, while region, gender, age, and user-segment performance is not separately supplied because those settings act as ad-selection hints.
- Official source checked 2026-07-30: https://ads.naver.com/notice/32709

### 2) 기존 지식에서 수정할 점

- The uploaded August media report says the AI agent rewrites copy and `결정 가격을 성과에 맞춰` 운영한다고 요약했지만, client wording should remain more precise: advertisers cannot set a separate ADVoost Max bid, and CPC is determined by Naver's stated ADVoost Max pricing logic rather than by a freely editable AI bid.
- Do not describe demographic/location settings as strict exclusion or guaranteed targeting controls for ADVoost Max. They are hints and do not produce a separate targeting-level report.
- Do not leave the default ON setting unchecked during account takeover. Review every expanded-search ad group before spending begins.

### 3) 실무 적용 원칙

1. Audit all expanded-search ad groups for ADVoost Max ON/OFF status.
2. Check landing-page text, business information, schema, conversion scripts, and all URLs inside the ad group because AI-written copy and URL selection rely on account and landing information.
3. Use the dedicated ADVoost Max Insight report and compare it with the aggregate management-screen figure.
4. If control, report granularity, or industry eligibility is insufficient, keep ADVoost Max OFF for that ad group and test only after prerequisites are corrected.

### 4) 제안서/리포트 문장 예시

> ADVoost Max는 AI 브리핑 문맥과 랜딩페이지 정보를 바탕으로 광고 문안과 연결 대상을 판단하는 확장형 검색광고입니다. 기존 확장검색 광고그룹은 기본 ON 여부를 먼저 점검하고, 전용 인사이트 보고서에서 실제 노출 문안과 성과를 확인한 뒤 유지 여부를 결정하겠습니다.

### 5) 다음 확인 필요사항

- Current restricted-industry list and account-level eligibility.
- Final pricing description and any later changes to CPC calculation.
- Whether insight-report fields, update frequency, or targeting hints change after launch stabilization.
