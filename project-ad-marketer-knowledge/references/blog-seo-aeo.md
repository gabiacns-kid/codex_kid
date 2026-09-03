# Blog SEO/AEO Audit and Writing Reference

Use this reference when the user asks for SEO/AEO blog drafts, blog content audits, SEO diagnosis files, technical SEO checklists, schema markup guidance, or AEO/GEO-style content optimization.

## Current Official Baseline

- Treat AEO/GEO as an extension of SEO, not a replacement. Google states that generative AI features in Search rely on the Search index, ranking, quality systems, RAG, and query fan-out. Therefore crawlability, indexability, snippets, content quality, and technical SEO remain the base.
- Correct outdated Core Web Vitals language: use **LCP, INP, CLS**. Do not use FID as the current responsiveness metric unless explaining older reports.
- Do not promise rich results. Structured data gives eligibility and clearer machine understanding; it does not guarantee rich result exposure.
- Be careful with FAQPage claims. Google removed/deprecated FAQ rich results in Search in 2026, so FAQ still helps structure, user clarity, and AI-readability, but should not be sold as a guaranteed Google FAQ rich result tactic.
- Structured data must describe visible page content. Do not add schema for hidden, invented, outdated, or mismatched information.

## Audit Response Workflow

When the user uploads an SEO/AEO diagnosis file or asks for a revision direction, respond in this order:

1. **Separate severity**: critical crawl/index issues, high-impact snippet/content issues, AEO structure improvements, optional polish.
2. **Explain why it matters**: search exposure, AI answer eligibility, snippet quality, trust, CTR, or technical crawl efficiency.
3. **Give concrete fixes**: exact meta tag, content rewrite direction, schema type, page-level action, or validation tool.
4. **Flag unverifiable items**: items requiring GSC, Naver Search Advisor, CMS access, page source, server settings, or live crawling.
5. **Avoid overclaiming**: say "노출 가능성/해석 가능성 개선" rather than "상위노출 보장" or "AI 답변 인용 보장".

## SEO Technical Checklist

### Crawl and Index

Check:

- Google Search Console and Naver Search Advisor registration.
- `sitemap.xml` exists, is submitted, and reflects canonical important URLs.
- `robots.txt` does not block important pages, CSS, JS, images, or API-rendered content needed for rendering.
- Canonical tags are present and do not point to irrelevant duplicates.
- Important pages return 200 status and are not `noindex`.

Fix direction:

- Submit or update sitemap.
- Remove accidental robots/noindex blocks.
- Fix canonical mismatch.
- Request re-indexing only after the page is technically correct.

### HTTPS and Internal Links

Problem:

- HTTPS pages containing HTTP internal links or resources can cause redirects, mixed-content issues, and inefficient crawling.

Fix direction:

- Convert internal absolute links and resource URLs to HTTPS.
- Prefer relative URLs or canonical HTTPS host rules where appropriate.

### Mobile and Page Experience

Check:

- Mobile viewport meta tag exists: `<meta name="viewport" content="width=device-width, initial-scale=1">`
- Layout is readable and clickable on mobile.
- Core Web Vitals use current metrics: LCP under 2.5s, INP under 200ms, CLS under 0.1 as target thresholds.

Fix direction:

- Add viewport tag.
- Compress large images, improve server response, reduce render-blocking assets, reserve image/layout dimensions, and test with PageSpeed Insights and GSC Core Web Vitals.

### Open Graph and Social Preview

Check:

- `og:title`, `og:description`, `og:image`, `og:url`, and relevant Twitter/X card tags.

Fix direction:

- Add page-specific OG tags so shared links in KakaoTalk, social channels, and messenger previews show the correct title, description, and image.

## On-Page SEO Checklist

### Title

Use:

- Unique page-level `<title>`.
- Descriptive and concise wording.
- Primary keyword near the front when natural.
- Avoid keyword stuffing, repeated boilerplate, and vague titles like "Home".
- Keep Korean blog titles practical; length is not a fixed rule, but long titles may truncate.

Audit wording:

> 현재 제목은 핵심 키워드가 후방에 있거나 페이지 고유성이 약합니다. 검색 결과와 AI 요약에서 주제를 즉시 파악할 수 있도록 핵심 키워드를 전면에 두고, 페이지별 차별 문구를 추가하는 방향이 좋습니다.

### Meta Description

Use:

- Unique description for each important page.
- Human-readable summary that reflects the page content.
- Avoid keyword lists and duplicated boilerplate.
- Include decision-useful information such as service area, price basis, product type, eligibility, benefit, or comparison point when visible in the page.

Audit wording:

> 메타 디스크립션은 검색 결과 스니펫의 후보가 되는 요약 정보입니다. 현재 설명문이 중복되거나 추상적이라면, 페이지별 핵심 답변과 차별점을 1~2문장으로 재작성하는 것이 좋습니다.

### Alt Text

Use:

- Describe the actual image and context.
- Include useful product/service terms only when natural.
- Avoid meaningless file names, keyword stuffing, and repeated identical alt text.

Example:

- Weak: `banner01`
- Better: `사무용 책상과 의자를 함께 배치한 6인 오피스 가구 세트`

## AEO Content Design

### Answer-First Structure

For informational pages and blog posts:

- Put the answer or conclusion near the top.
- Use a short "핵심 요약" block.
- Use H2/H3 headings that mirror real user questions.
- Write each section so it can stand alone as a useful answer passage.
- Prefer tables, bullet lists, process steps, and comparison criteria.

### Long-Tail and Persona Questions

Do not only target short keywords. Add natural-language questions:

- "소규모 병원은 네이버 검색광고 예산을 어떻게 잡아야 하나요?"
- "B2B 판촉물 제작 업체는 파워링크와 파워컨텐츠 중 무엇이 먼저인가요?"
- "자사몰 없이 메타 광고를 진행하면 전환 측정이 가능한가요?"

For B2B, map questions by:

- Decision maker: cost, risk, vendor reliability.
- Practitioner: process, setup, tools, comparison.
- Buyer stage: problem recognition, vendor comparison, quote request, execution.

### FAQ Section

Use FAQ for user clarity and answer extraction, not as a guaranteed Google FAQ rich-result tactic.

Good FAQ:

- 5 to 7 related questions per core topic.
- First sentence gives a complete answer.
- 2 to 4 concise sentences per answer.
- Include numbers, conditions, caveats, or examples where true.
- Keep all FAQ content visible on the page if using FAQPage schema.

## E-E-A-T for AEO

Add signals that make the content harder to replace with generic AI text:

- **Experience**: actual client cases, audit observations, test results, operating lessons, failure cases.
- **Expertise**: specific metrics, comparison criteria, implementation steps, policy caveats.
- **Authoritativeness**: official sources, credible third-party data, expert author or company credentials.
- **Trustworthiness**: updated date, scope limits, assumptions, limitations, transparent risks.

Audit wording:

> 내용은 맞지만 일반론에 가깝습니다. AI 답변에 인용될 가능성을 높이려면 실제 운영 경험, 수치, 비교 기준, 주의사항을 넣어 '누구나 쓸 수 있는 설명'에서 '이 업체가 직접 판단한 정보'로 바꿔야 합니다.

## Structured Data / Schema

### General Rules

- Prefer JSON-LD.
- Insert in `<head>` or before `</body>`.
- Use Google Search Central documentation as the source for Google Search behavior.
- Validate with Rich Results Test and Schema.org validator.
- Monitor with Google Search Console where available.
- Schema must match visible page content.
- Avoid mixed formats unless there is a clear reason.
- Keep price, availability, rating, business info, and FAQ synchronized with the page.

### Common Types

| Page type | Candidate schema | Notes |
|---|---|---|
| Product detail | `Product`, `Offer`, `AggregateRating` | Use only for actual product page. Keep price and availability current. |
| Organization home | `Organization` | Include name, URL, logo, contact, sameAs where applicable. |
| Local business | `LocalBusiness` | Useful for store/location pages. Match visible address/contact. |
| Article/blog | `Article` or `BlogPosting` | Add author, datePublished/dateModified, headline, image. |
| FAQ content | `FAQPage` | Useful for structure, but do not promise Google FAQ rich result exposure. |
| How-to content | `HowTo` | Use only when the page contains actual visible step-by-step instructions and the feature is eligible/current. |

### Schema Audit Wording

> 구조화 데이터가 없으면 검색엔진과 AI가 페이지의 정보를 단순 텍스트로만 해석할 가능성이 높습니다. 다만 스키마는 노출을 보장하는 장치가 아니라 페이지 내용을 명확히 전달하는 기술적 보조 장치입니다. 우선 페이지 성격에 맞는 JSON-LD를 적용하고, 실제 화면에 보이는 정보와 일치하는지 검증해야 합니다.

## Blog Writing Output Format

When writing SEO/AEO blog content, return:

1. SEO title candidate.
2. Search-intent diagnosis.
3. Intro with direct answer.
4. Key summary.
5. H2/H3 structure.
6. Comparison tables where useful.
7. FAQ section.
8. Image/screenshot insertion points.
9. CTA.
10. Suggested tags.

## Critical Cautions

- Do not treat AEO as a shortcut that bypasses SEO.
- Do not create mass-produced question pages just to target AI query fan-out; this can look like scaled content abuse.
- Do not mark up invisible FAQ or product data.
- Do not promise AI citation, AI Overview inclusion, rich results, or ranking.
- Do not use outdated Core Web Vitals language unless the report itself is old.
- For current Google/Naver rules, verify official documentation before final advice.

## Official Sources To Recheck

- Google Search Central: Generative AI optimization guide.
- Google Search Central: Structured data introduction and general guidelines.
- Google Search Central: Core Web Vitals.
- Google Search Central: Title links.
- Google Search Central: Snippets/meta descriptions.
- Google Search updates: FAQ rich result deprecation/removal.
- Naver Search Advisor documentation when the target is Naver organic exposure.
