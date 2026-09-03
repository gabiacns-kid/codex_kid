# PPT and Proposal Artifact Guidance

Use this reference when creating GabiaCNS proposal PPTs or proposal documents.

## Purpose Types

### 1. Simple Sales Proposal

Use when the user asks for a working sales proposal deck.

- Build from the A-to-Z proposal logic.
- Choose design based on industry and purpose.
- Prioritize clarity, persuasive flow, and client-facing wording.
- Avoid excessive design experimentation.

### 2. Design Concept Reference

Use when the user asks for design references before building a detailed PPT.

- Create 3-4 different layout variations.
- Vary composition, structure, and visual hierarchy.
- The output is for the user's internal inspiration, not final client delivery.

## GabiaCNS PPT Baseline

- 16:9 only.
- Use Pretendard only.
- Keep title, subtitle, body styles consistent across slides.
- Do not use more than 5 font sizes unless there is a strong reason.
- Center text inside shapes vertically and horizontally.
- Use concise noun-phrase endings rather than long sentences.
- Increase line spacing for bullet lists.
- Do not leave the lower slide area empty.

For a clean, readable, unified performance-proposal deck similar to the WSE Naver proposal, use
`references/wse-clean-ppt-style.md`.

For a government-advertising RFP proposal deck similar to the 2026 H2 final qualitative proposal, use
`references/gov-ad-final-ppt-style.md`.

## Visual Safety Rules

PowerPoint file integrity is more important than decorative design.

Avoid fragile PptxGenJS patterns:

- Hex colors with `#`
- 8-digit hex shadows
- Reused shadow option objects
- Negative shadow offsets
- Unclear chevrons or unsupported arrow settings
- Text overflow inside small cards
- Text boxes touching footer zones

For fragile decks, prefer the last known working version and apply minimal fixes.

## Layout Quality Rules

- Every card should have at least title, sublabel, 2+ bullets, and a tag/status.
- KPI rows should use the full slide width evenly.
- Progress bars should reflect actual or intentionally assigned ratios, not identical decoration.
- Do not overuse green. Use green for section label, key KPI, or one accent only.
- Avoid green bullets; use gray dots or native bullets.
- Process boxes need explanatory text, not only titles.
- Rows/tags must contain readable text. Empty dark rectangles look broken.

## HTML Slide Layout Lessons

Apply these rules when producing PPT-style HTML slides or image-conversion decks.

- On cover slides, do not place bottom summary cards immediately beneath the subtitle. Reserve a clear vertical safety gap and move the card row farther down so it cannot cover the subtitle after font rendering.
- Treat a subtitle and its following card row as one collision-check group. Verify the rendered bottom edge of the subtitle before fixing the card-row position.
- For long Korean subtitles, do not rely only on automatic wrapping. Insert explicit line breaks at sentence boundaries, especially after periods and commas when the next phrase introduces a new idea.
- Keep each subtitle line semantically complete. A two- or three-line subtitle should read as short consecutive statements, not as arbitrary visual fragments.
- Apply the sentence-level line-break rule consistently across all slides, including opening diagnosis slides, strategy slides, and final action or landing-page slides.
- During visual QA, check cover-subtitle/card overlap and subtitle line structure separately from ordinary text overflow checks.

### Woowad Feedback, 2026-06-24

- Cover: the three summary boxes were too close to the subtitle and obscured it; lower the boxes.
- Slides 1, 3, and 10: break subtitles by sentence or clause at punctuation for clearer scanning.
- This feedback is retained for future production; the existing Woowad HTML deck does not need to be rebuilt.

## File Delivery Rule

Generated files should be placed under:

`C:\Users\GABIACNS\Documents\New project\생성파일`

Uploaded/reference files are usually under:

`C:\Users\GABIACNS\Documents\New project\업로드파일`

## Performance Proposal Completeness, 2026-07-24

- A performance-improvement PPT must preserve the full reasoning chain: `report evidence → funnel break → confirmed fact vs hypothesis → campaign/creative/site action → budget rationale → conditional expansion`.
- Do not compress a client-facing deck so far that it omits follow-on media plans, future audience use, current creative count and direction, learning disruptions, or attribution context when those points materially affect the recommendation.
- Every budget split must state why that ratio is appropriate using account evidence. A ratio without report-based logic is not a recommendation.
- When click-through rate and click cost look healthy but purchase efficiency is weak, show the purchase conversion rate, purchase cost, purchase revenue or ROAS, and the cart-to-purchase break together.
- Keep decorative section labels in Korean. Retain English only for official product names or unavoidable industry metrics such as GFA and GA4; prefer Korean terms for proposal, roadmap, targeting, traffic, CPA, and ROAS in advertiser-facing titles.
- A slide may be concise, but it must be independently readable. Avoid sparse fragments that require the presenter to supply the missing causal logic.
