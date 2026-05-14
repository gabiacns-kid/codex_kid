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
