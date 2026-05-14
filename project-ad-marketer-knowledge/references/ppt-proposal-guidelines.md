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

## File Delivery Rule

Generated files should be placed under:

`C:\Users\GABIACNS\Documents\New project\생성파일`

Uploaded/reference files are usually under:

`C:\Users\GABIACNS\Documents\New project\업로드파일`
