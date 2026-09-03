# Proposal Production Pipeline

Use this reference when the user asks for a complete Korean online advertising proposal workflow, especially when the work includes strategy, advertiser data analysis, Word proposal writing, and PPT production.

## Core Direction

The proposal should not start from a channel list or a design template. Start from the advertiser's business problem and build a practical operating strategy. If the advertiser provides data, use it as the evidence layer that explains why the strategy is necessary.

Default proposal logic:

1. Define the advertising objective and conversion path.
2. Establish the operating strategy at a high level.
3. Analyze advertiser data if available.
4. Map the operating strategy onto the actual issues found in the data.
5. Define KPI direction and target scenarios.
6. Add relevant references or comparable performance cases.
7. Write a detailed Word proposal.
8. Convert the Word proposal into a concise, visually consistent PPT.

## Critical Thinking Gate

Before producing materials, challenge the user's or source document's logic.

- Does the proposed media plan have enough budget and data volume to optimize?
- Is the KPI realistic for the advertiser's funnel and average revenue?
- Is the proposal solving the advertiser's problem, or only listing available ad products?
- Are supporting media framed as limited validation tests rather than broad expansion?
- Are claims about ROAS, CPL, CPA, or conversion improvement connected to an operating mechanism?
- If data is missing, is the gap clearly stated as a confirmation item rather than hidden?

If the logic is weak, correct it and propose stronger client-facing wording.

## Data-Based Diagnosis

When advertiser data is available, use it to create the proposal's evidence layer.

Minimum checks:

- Spend, sales, ROAS, CPA, CPL, CPC, CTR, impressions, clicks.
- Funnel conversion: click to lead, lead to show/visit/consultation, show to contract/registration.
- Campaign/ad group/keyword contribution by spend, leads, contracts, ROAS, and CPA.
- High-cost low-conversion groups.
- Low-rank or low-volume but high-quality groups.
- Lead volume versus lead quality.
- Whether total rows and detail rows are both present; avoid double counting.

For lead-generation proposals, do not stop at CPL. Evaluate the full path:

`Click -> Lead submission -> Show/visit/consultation -> Contract/registration -> Sales/ROAS`

Use the advertiser's own CRM, BI, HubSpot, Power BI, or sales data where available. If only ad-platform data is available, state that lead quality and revenue contribution must be confirmed separately.

## Strategy Application

After diagnosing the current state, translate findings into operating actions.

Recommended mapping:

| Data signal | Operating interpretation | Proposal action |
|---|---|---|
| High spend, low ROAS | Cost is being consumed before quality is proven | Rank/bid control, max-bid guardrail, keyword regrouping |
| High click volume, low lead rate | Search intent or landing message mismatch | Keyword intent split, ad copy test, landing-page test |
| High lead volume, low contract rate | Lead quality issue | CRM/BI feedback, lead-quality scoring, budget reallocation |
| High conversion rate, low volume | Expansion candidate | Rank-up test, budget increase, similar keyword expansion |
| Broad/expanded search terms mixed with quality terms | Control precision is weak | Discovery -> performance selection -> direct keyword registration -> rank management |

Do not present optimization as one-time correction. Present it as a repeatable operating loop.

## KPI Direction and Target Scenarios

KPI targets should be calculated from the advertiser's actual funnel where possible.

For each stage, calculate:

- Click to lead rate.
- CPL.
- Lead to show/visit rate.
- Cost per show/visit.
- Show/visit to contract rate.
- CPA.
- Average revenue per contract.
- ROAS.

Then build scenarios:

- Current baseline.
- Minimum acceptable target.
- Healthy target.
- Aggressive target.

For ROAS, do not overpromise. Explain that the proper target depends on margin, sales labor cost, refund/cancellation, and LTV. If margin is unknown, present ROAS as a directional performance target and list margin/LTV as confirmation items.

## Reference and Case Study Layer

Use references after the strategy and data diagnosis, not before them. The reference should prove that the proposed operating method is realistic.

Case studies should be anonymized if the client name cannot be disclosed.

Preferred structure:

- Industry type instead of company name.
- Before/after period such as "before improvement" and "after improvement, 90 days."
- Core result: cost, CPC, clicks, leads, CPA, conversion rate, ROAS where available.
- How-to: bid/rank control, max-bid management, keyword expansion, waste reduction, landing/creative test, lead-quality feedback.
- Why it is relevant to the current advertiser.

## Word Proposal First

For complex proposals, write the Word version before the PPT.

The Word document should contain:

- Detailed diagnosis and interpretation.
- KPI calculations and assumptions.
- Data tables and operating judgement.
- Strategy explanation.
- Confirmation items.
- Internal or presenter notes when needed.

Create separate versions when necessary:

- Client-facing KR version.
- Client-facing EN version.
- Internal/presenter version with script or extra notes.

## PPT Conversion

The PPT should not simply paste the Word content. Convert each Word section into one clear slide job.

Default PPT flow:

1. Proposal title and core promise.
2. KPI/funnel frame.
3. Data snapshot or current-state diagnosis.
4. Main performance insight.
5. Account/search structure strategy.
6. Operating system or improvement loop.
7. Core solution such as DIAD Pro or auto-bidding.
8. Supporting media/test strategy.
9. Measurement and reporting.
10. Budget or KPI target direction.
11. Case studies.
12. Team/resource structure.
13. Closing.

PPT rules:

- Use the same story order as the Word proposal.
- Keep slide wording shorter than Word wording.
- Keep visual hierarchy consistent across KR and EN versions.
- Preserve agreed fonts, font sizes, colors, and layout rules.
- Do not add new claims in PPT that are not supported by the Word or source data.
- When translating, use advertising-domain language, not literal translation.

## Design and File QA

For PPT/DOCX production, preserve the user's chosen format unless asked to redesign.

Check before delivery:

- Same section order across Word and PPT unless intentionally different.
- No missing core strategy section.
- No leftover internal-only notes in client-facing files.
- No unsupported product claims or outdated platform terms.
- No typo in brand/service names such as DIAD Pro.
- No PowerPoint repair-warning risk from broken XML, duplicate package entries, or missing relationships.
- For Excel-based analysis, avoid double counting total rows and detail rows.

## 2026-09-03 변경 요약: 사용자 편집본 보존과 부분 수정 원칙

### 1) 새로 학습한 사실

- 사용자가 Word에서 직접 수정한 문서를 생성 스크립트로 같은 파일명에 다시 저장하면, 자동복구·임시 사본·파일 기록이 없는 환경에서는 이전 편집 내용을 복구하지 못할 수 있다.
- 문서 생성 스크립트가 오래된 초안을 기준으로 전체 문서를 재생성하면 요청한 한 개 항목만 고쳐도 사용자가 다른 항목에 반영한 수정사항이 함께 사라질 수 있다.

### 2) 기존 지식에서 수정할 점

- `빌더를 고친 뒤 동일 파일을 재생성`하는 방식을 사용자 편집본의 기본 수정 절차로 사용하지 않는다.
- 현재 문서가 사용자가 직접 검토·수정한 버전인지 확인하지 않은 채 작업용 스크립트를 진실의 원본으로 간주하지 않는다.
- 부분 수정 요청을 전체 문서 재생성으로 처리하지 않는다.

### 3) 실무 적용 원칙

1. 수정 전 현재 사용자 편집본을 읽고 별도 이름의 백업 사본을 만든다.
2. 사용자가 요청한 구간만 기존 DOCX에 직접 패치하고, 원본과 다른 새 버전 파일명으로 저장한다.
3. 전체 재생성이 꼭 필요하면 현재 문서의 문장·표·서식과 빌더 결과를 먼저 비교하고 사용자의 편집사항을 빌더에 역반영한 뒤 실행한다.
4. 수정 후에는 요청 구간 외 문장과 표가 바뀌지 않았는지 구조 비교를 하고, 실제 렌더링으로 페이지·표·서식을 검수한다.
5. 사용자 편집본, 수정 전 백업, 최종 수정본을 구분해 보관하며 최종 확인 전 기존 파일을 덮어쓰지 않는다.

### 4) 제안서/리포트 문장 예시

> 현재 검토본을 원본으로 보존한 뒤 요청하신 항목만 수정해 새 버전으로 저장하겠습니다. 수정 구간 외 문장과 표는 비교 검수하여 기존 편집사항이 유지되도록 하겠습니다.

### 5) 다음 확인 필요사항

- 사용자 편집본의 기준 파일명과 최종 저장 시각
- Word 자동저장·OneDrive 버전 기록·Windows 파일 기록 사용 여부
- 수정 전후 DOCX 문단·표 비교를 자동화할 수 있는 검수 절차
- 최종본 확정 전 백업 파일의 보존 기간과 폴더 규칙

## Client-Facing Summary Pattern

Use this pattern when summarizing the proposal:

> We first define the operating strategy, then diagnose the advertiser's current data, apply the strategy to the actual issues found in the account, and set KPI targets and reference evidence. The Word document contains the detailed logic, while the PPT turns that logic into a concise client-facing proposal flow.
