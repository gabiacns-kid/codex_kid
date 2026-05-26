# WSE Clean Proposal PPT Style

Use this reference when the user asks for a clean, readable, unified, professional PPT style similar to the WSE Naver PowerLink proposal deck.

This is a proposal style for serious B2B advertising meetings. It should feel clear, structured, and evidence-led rather than decorative.

## Design Intent

- The deck should look like a polished consulting-style operating proposal, not a marketing brochure.
- Prioritize readability, data interpretation, and logical flow.
- Use consistent structure slide to slide, but vary the content layout enough to avoid monotony.
- Keep one clear job per slide: KPI frame, data snapshot, operating insight, solution, test system, reporting, reference, or team input.
- Design should support the argument. Do not add decorative elements that do not clarify the proposal.

## Visual System

Use a restrained white-background system.

Core colors:

| Role | Color | Use |
|---|---|---|
| Background | `FFFFFF` | Main slide background |
| Primary text | `181818` or `0D1F0D` | Main titles and strong labels |
| Body text | `303030` | Body copy |
| Secondary text | `666666` or `888888` | Captions, helper copy, footers |
| Line/divider | `CCCCCC` | Thin rules, card boundaries, subtle separation |
| Primary accent | `1EC800` | Section labels, KPI accents, key tags |
| Deep green accent | `17A300` | Secondary accent, status markers |
| Limited blue accent | `2F6BFF` | Rare data emphasis only |
| Pale blue-gray | `DDE5EF` | Quiet background fill for small emphasis zones |

Do not overuse green. Green should work as a navigation/accent signal, not a full-page theme.

## Typography

Use Pretendard as the default font. Keep typography consistent.

Recommended type scale:

| Role | Size |
|---|---:|
| Cover title | 36-40 pt |
| Main slide title | 26-28 pt |
| Card/section title | 18 pt |
| Body | 15 pt |
| Small body / table text | 11-12 pt |
| Footer / label / tag | 8-10 pt |

Use SemiBold only for titles, section labels, and KPI labels. Avoid too many weights.

## Page Structure

Default slide layout:

- Top-left section label: small uppercase or numbered label such as `02 / DATA INSIGHT`.
- Large title under the label.
- One subtitle line under the title.
- Main content from roughly the upper-middle to lower-middle of the slide.
- Footer line at the bottom with deck name and company name.
- Maintain generous side margins of around 0.5 inch.

The style works best when title and subtitle are left-aligned and the main content fills the width evenly.

Avoid:

- Center-heavy title-only pages except section dividers.
- Dense paragraphs inside large boxes.
- Cards that leave the lower half empty.
- Text boxes touching the footer area.
- Random icon decoration.

## Common Slide Patterns

### 1. Three-Stage KPI Frame

Use for funnel strategy.

Structure:

- Three equal columns.
- Each column has a small number label, KPI title, funnel stage, and 2-3 operating levers.
- Use thin dividers or arrows between columns.
- Add one bottom note explaining the core view.

Good for:

- CPL / CPA / ROAS connection.
- Click -> Lead -> Show -> Contract flow.

### 2. Four-KPI Snapshot

Use for current performance.

Structure:

- 2x2 KPI blocks.
- Each block includes label, title, main number, and 1-2 interpretation lines.
- Add a bottom interpretation statement.

Good for:

- Cost, Sales, Leads, Contracts.
- CPL, CPA, ROAS, Lead-to-Contract.

### 3. Four-Quadrant Insight Grid

Use for keyword type or campaign insight.

Structure:

- 2x2 cards.
- Each card has a short green tag, title, metric line, and operating direction.
- Add a bottom `Operating Decision` or `Implication` band.

Good for:

- General, Online/OCC, Region/Center, Consultation/Level Test.
- Scale, maintain, adjust, test groups.

### 4. Operating System Slide

Use for long-term strategy.

Structure:

- 4-5 operating axes arranged evenly.
- Include feedback loop or data-feedback badge.
- End with one summary statement that says the items work as one repeatable system.

Good for:

- Search intent structure.
- Rank efficiency.
- Landing/conversion path.
- Information touchpoints.
- Performance data feedback.

### 5. Solution Slide

Use for DIAD Pro, automated bidding, or core operating tools.

Structure:

- Title positions the solution as an operating infrastructure, not a magic performance guarantee.
- 3-4 small modules with KPI effect.
- Bottom differentiator statement.

For DIAD Pro, always mention rank monitoring, automated bid adjustment, max-bid control, bid history, and CPC efficiency.

### 6. Test System Slide

Use for A/B testing.

Structure:

- Divide tests by purpose: click improvement and conversion improvement.
- Include data sources: Naver Ads, HubSpot, Power BI.
- Include test objects: keyword, rank, bid, creative, landing, conversion path, expanded search.

Do not make A/B testing sound like copy-only testing.

### 7. Reporting Slide

Use for collaboration and reporting.

Structure:

- Weekly report, monthly report, real-time issue response.
- One metric-standard row.
- Use practical metric labels such as Imp, Click, CTR, CPC, CVR, CPL, CPA, ROAS, Lead, Show, Contract.

### 8. Reference Case Study Slide

Use for before/after performance.

Structure:

- Industry label, not client name, when anonymized.
- 4-5 KPI tiles.
- Short `How to` or `Application to WSEKR` section.
- Keep the case as proof of operating method, not as unrelated bragging.

## Wording Rules

Use concise, professional English. Avoid literal Korean translation.

Preferred wording:

- `Performance Improvement Strategy`
- `Operating System`
- `Performance Snapshot`
- `Operating Decision`
- `Lead Quality`
- `Supporting Media`
- `Limited Validation Test`
- `Resource Allocation Structure`
- `Automated Bidding`
- `Rank Management`
- `Max-Bid Control`
- `Show (consultation attendance)` on first use

Avoid:

- `Operational Advancement Strategy`
- `Advanced Performance Operation Strategy`
- `Not Jus Position defense`
- `Ab testing`
- `Power contents`
- `DIAD pro`
- `Kakao Brand Messages` when referring to the product name; use `Kakao Brand Message`
- Overly broad claims such as "build a powerful campaign" without KPI logic.

## English QA Rules

Before delivery, scan for:

- DIAD Pro capitalization.
- PowerLink and Power Content spelling.
- Kakao Brand Message singular product name.
- Contract capitalization when it is used as the WSE final conversion stage.
- First-use definition of Show if foreign stakeholders will read the deck.
- Broken sentence joins such as `CPCAfter`.
- Typos such as `coast`, `congidentially`, `busuness`, `mus`.
- Awkward phrases caused by direct translation.

## File QA Rules

Before delivering a PPT, check:

- Slide count and section order.
- Duplicate ZIP/package entries.
- XML parse errors.
- Missing internal relationships.
- No text overflow near footer.
- No accidental decorative symbols or unsupported characters caused by export.

If a deck was previously repaired by PowerPoint, do not keep editing blindly. Inspect package structure and relationships before delivering.
