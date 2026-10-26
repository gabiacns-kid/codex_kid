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

## 2026-09-22 변경 요약: AI 문체 억제와 보고서 시각 위계

### 1) 새로 학습한 사실

- 실무 리포트에서 `A가 아니라 B`, `핵심은 ~에 있습니다` 같은 대조·격언형 종결이 반복되면 AI 문체로 인식되기 쉽다.
- `따라서`, `반대로`, `다만`, `가능성이 큽니다`, `구조`를 여러 섹션에서 반복하면 내용이 맞아도 기계적인 인상을 준다.
- 핵심 요약과 최종 결론이 같은 진단을 반복하면 결론의 역할이 약해진다. 첫머리는 판단 기준, 마지막은 실행 순서·확인 자료·중단 조건으로 역할을 나눈다.
- 표가 많은 PDF는 모든 표를 같은 회색 톤으로 처리하면 우선순위를 파악하기 어렵다. 핵심 진단, 우선 실행, 최종 액션과 표의 역할군에 서로 다른 제한된 색을 적용한다.

### 2) 기존 지식에서 수정할 점

- 근거 수준은 문단마다 `사실과 추론`을 설명하지 않고, 표 각주·자료 적용 기준·확인 필요 표시로 짧게 구분한다.
- 모든 문장을 헤지 표현으로 끝내지 않는다. 자료로 확인된 값과 실행 제안은 단정문으로 쓰고, 미확인·가정·변동 가능 항목만 조건부 표현을 사용한다.
- 블로그형 소제목보다 `베스트 상품의 시사점`, `검색수요 불일치 항목`, `고검색량·검증 필요 키워드`처럼 업무 내용을 바로 보여주는 제목을 사용한다.

### 3) 실무 적용 원칙

1. 대조구문은 실제 반전이나 비교가 필요한 1~2곳만 남긴다.
2. 같은 접속사와 추상명사를 반복 검색해 절반 이상 삭제하거나 문장을 직접 연결한다.
3. 요약은 핵심 진단과 판단 근거를, 결론은 1~2주차 실행 항목과 확인할 데이터를 제시한다.
4. 긴 보고서는 강제 페이지 나누기를 최소화하고, 표 행 분할 금지·차트 색상 통일·핵심 수치 시각화를 렌더링 결과에서 점검한다.
5. 데이터 표가 많은 경우 `요약 PDF + 필터·정렬 가능한 데이터 워크시트` 구성을 선택지로 제안하되, 사용자 요청 범위를 넘어 자동 생성하지 않는다.

### 4) 제안서/리포트 문장 예시

> 1~2주 내 상품별 마진과 주문 조합을 확인한 뒤 하이박스·LED십자등 캠페인부터 시작합니다. 저가 부자재는 단독 광고 대상보다 연관 구매와 객단가 기여도를 기준으로 평가합니다.

### 5) 다음 확인 필요사항

- 최종 전달 형식이 의사결정용 PDF인지 운영용 데이터 문서인지
- 페이지별 정보 밀도, 표 행 분할, 차트 색상, 핵심 수치 강조가 실제 렌더링에서도 유지되는지
- 단정문으로 바꾼 표현이 공개 자료의 확인 범위를 넘어 확정 사실처럼 보이지 않는지

## 2026-09-30 변경 요약: 광고주용 문서의 표 서식과 정보 선별 기준

### 1) 새로 학습한 사실

- 광고주용 Word 문서의 표마다 글자 크기가 달라지면 같은 문서 안에서도 완성도가 떨어져 보인다. 폰코니 최종 편집본은 12개 표의 본문 글자를 모두 8.5pt로 통일하고 모든 셀 문단을 가운데 정렬했다.
- 조사 출처, 공식 문서 확인 과정, API 제공 상태처럼 분석의 신뢰성을 내부적으로 검증하는 정보라도 광고주의 의사결정과 운영에 직접 필요하지 않으면 제안서 본문에서 제외하는 편이 낫다.
- 사용자가 직접 고친 최종본은 문장 톤, 페이지 분리, 강조 방식과 정보 밀도를 보여주는 우선 참고본이다. 생성 스크립트의 초안보다 최종 편집본의 선택을 먼저 따른다.

### 2) 기존 지식에서 수정할 점

- 표 크기는 내용량에 따라 임의로 8pt, 8.5pt, 9pt를 섞지 않는다. 한 문서 안에서는 동일한 표 글자 크기를 유지한다.
- 표 글자는 기본 9pt로 작성하고, 정보량 때문에 축소가 꼭 필요할 때만 문서 전체 표를 8.5pt로 통일한다. 8.5pt 미만은 사용하지 않는다.
- 출처와 공식 문서 검증 내용은 내부 근거 자료에 남기되, 광고주용 문서에는 정책·기능·한계가 실제 운영 판단에 영향을 줄 때만 짧게 설명한다. 별도 출처 장은 광고주나 제출 요건이 요구할 때만 넣는다.

### 3) 실무 적용 원칙

1. 문서 생성 전 표 본문 글자 크기를 하나로 정하고 모든 표에 동일하게 적용한다. 권장값은 9pt, 최소값은 8.5pt다.
2. 표 제목 행과 본문 셀의 문단은 모두 가로·세로 가운데 정렬한다. 설명이 긴 표라도 정렬 기준을 임의로 바꾸지 않는다.
3. 광고주용 본문에는 광고 운영 결정, 예산, 상품, 타겟, 소재, 측정, 실행에 필요한 내용만 남긴다. 조사 과정·API 기술 설명·공식 문서 검증 내역은 내부 검수 자료로 분리한다.
4. 문장을 사용자의 기존 표현과 용어에 맞추고, `A가 아니라 B`, 격언형 결론, 과도한 대조, 추상적인 `구조·시그널·레버리지`, 반복 접속사와 과도한 헤지 표현을 최종 검수에서 줄인다.
5. 사용자 편집본이 있으면 표 글자 크기, 셀 정렬, 강조 색상, 페이지 나누기와 삭제된 항목을 먼저 분석해 이후 같은 유형의 문서에 적용한다.
6. 납품 전 모든 표의 글자 크기와 정렬을 구조적으로 검사하고, 전체 페이지를 렌더링해 표 넘침·가독성·페이지 균형을 확인한다.

### 4) 제안서/리포트 문장 예시

> 광고는 구매 구성이 명확한 상품부터 시작하고, 저가 낱개 상품은 실제 광고 반응과 주문당 광고비를 확인하면서 운영 범위를 조정합니다.

### 5) 다음 확인 필요사항

- 광고주가 출처 표기를 요구하는 공공기관·입찰·정책 제안서의 예외 기준
- 표가 많은 데이터 부록을 본문과 별도 파일로 분리할지 여부
- 새로운 사용자 편집본에서 반복적으로 채택되는 문장과 강조 방식

## 2026-10-23 시연형 B2B AI 제품의 초기 미디어믹스

### 1) 새로 학습한 사실

- 알고리즘랩스 사례의 사용자 제공 조건: AI Blueprint 시연 시 반응이 크며 대기업·중견기업 AX·IT기획 담당자가 목표. 월 400만 원은 네이버 200만 원, Meta 100만 원, Google 100만 원으로 제안된 상태다. 이를 다른 광고주의 성과 근거로 일반화하지 않는다.
- 공개 홈페이지 https://algorithmlabs.ai/ 확인: 메인 설명과 시연은 AI Canvas 중심이며 Blueprint는 Plan, Canvas는 Build, Tower는 Management로 제시된다. 제품 간 효과·인증·실적 수치를 옮겨 쓰지 않는다.
- 네이버 https://ads.naver.com/help/faq/924 (2026-09-16 수정, 2026-10-23 확인): ADVoost 오디언스는 시그널 외 이용자에도 노출될 수 있고 모든 지원 게재위치 선택 등 제약이 있다. 특정 기업·직무 제한 기능으로 설명할 수 없다.

### 2) 기존 지식에서 수정할 점

- 홍보 비중이 크다는 요구를 모든 DA 캠페인의 조회·트래픽 목표로 치환하지 않는다. 시연 콘텐츠로 설명하되 Meta 웹사이트 잠재 고객 캠페인처럼 신청을 목표로 하는 방식을 함께 검토한다.
- 상담 신청 완료와 실제 대상 기업의 상담 가능 문의는 별도 지표다. 직무 타겟 옵션 또는 AI 관심 신호가 실제 재직·구매 권한을 입증하지 않는다.

### 3) 실무 적용 원칙

- 제품별 랜딩의 주제가 광고와 일치하는지 먼저 본다. 회사 메인이 다른 제품 중심이면 기존 사이트 안의 제품 전용 페이지를 제안한다.
- 저예산 복수매체는 핵심 운영 단위만 만들고, 표본 부족이 지속될 경우 매체를 줄이는 조건을 포함한다. 구체적 예산 비율은 제안 가정으로 명시한다.
- 검색량이 작으면 무관한 일반 키워드로 소진하지 않는다. 설명형 매체의 시연을 보강하거나 다음 기간에 광고상품을 교체한다.
- 실제 데모 입력·결과물·제공 범위를 보여주고 보안 자료나 고객 사례는 승인된 범위만 사용한다.
- 최신 투자액·상장 일정·인증이 자료마다 다르면 최신 승인 문구를 받기 전 광고에서 제외한다. 상장 준비를 서비스 구매 전환의 증거로 쓰지 않는다.

### 4) 제안서 문장 예시

> 초기에는 시연을 통한 제품 이해와 검색 수요 확보를 함께 진행합니다. 첫 달의 문의 품질을 확인하고, 표본이 부족한 매체는 다음 달에 예산을 집중하는 방향으로 조정합니다.

### 5) 다음 확인 필요사항

- 실제 검색량·CPC·제품 데모 범위·상담 처리 기간·태그 정상 수집 및 매체 계정의 선택 가능 설정.
- Meta 공식 페이지는 이번 확인에서 로그인 차단으로 최신 본문 검증 미완료. 기존 공식 도움말 기반 지식과 실제 계정 확인을 병행해야 한다.
- Google 검색·PMax 선택 근거: https://support.google.com/google-ads/answer/2567043 ; 키워드 의미 매칭: https://support.google.com/google-ads/answer/14996023 . 2026-10-23 확인.
