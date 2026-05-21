# PPT 복구 메시지 QA 메모

WSE/GabiaCNS PPT 수정 시 PowerPoint 복구 메시지가 발생한 이력이 있으므로, 이후 PPT 생산/수정에서는 아래 항목을 기본 점검한다.

- 복구 메시지가 발생한 경우, 사용자가 PowerPoint에서 복구 후 저장한 파일을 새 기준 파일로 삼는다.
- ZIP 수준의 슬라이드 삽입은 가급적 피하고, 기존 PPT 내부에서 확인된 슬라이드/레이아웃을 기준으로 수정한다.
- PPTX 수정 후 `presentation.xml`, `presentation.xml.rels`, `[Content_Types].xml`, `slide*.xml.rels`의 누락 관계를 점검한다.
- 원본 생성본과 복구본을 슬라이드 순서 기준 텍스트로 비교해 삭제/변경된 가시 콘텐츠를 확인한다.
- 새 슬라이드 추가 시 기존 배경, 폰트 크기, 하단 정리 문구 구조, 푸터 체계를 반드시 맞춘다.
