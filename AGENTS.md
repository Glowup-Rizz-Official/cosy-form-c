# AGENTS.md

이 저장소에서 일하는 사람과 코딩 에이전트가 먼저 읽는 문서다. 지금은 작업 일감 규칙만 둔다.

## 작업 일감(ERP)

- 작업은 ERP 일감에서 시작한다. ERP MCP(`erp`)로 같은 일감이 있는지 먼저 찾고(`erp_ticket_list`), 없으면 COSY 그룹(앞머리 `COSY`)에 만든다(`erp_ticket_create`, PR 을 나누면 `erp_subtask_create`). 조회에 실패하면 "없음"으로 보지 않고 번호를 지어내지 않는다.
- 작업 브랜치 이름은 `종류/번호`다(예: `feat/COSY-12`). 번호 뒤에 설명을 붙이지 않는다. 유지 브랜치(`main`, `dev` 등), `release/`, 충돌 해결용 통합 브랜치는 대상이 아니다.
- PR 제목 끝에 같은 번호를 붙인다(예: `feat: 배송지 삭제 기능 추가 (COSY-12)`).
- 일감 본문에 무엇을, 왜, 어디를 바꾸는지 적는다. 데브봇이 이 본문과 PR 변경 파일로 개발 일감 등급을 매긴다.
- ERP MCP 는 개인 ERP 계정으로 로그인한다. 에이전트 계정은 공용이라 개인 계정이어야 본인 이름으로 일감이 생긴다.

규칙 정본은 [팀 규칙 TEAM-25](https://github.com/Glowup-Rizz-Development/team-standards/blob/main/AGENTS.md#gitpr), 연결 방법은 [ERP MCP 연결](https://github.com/Glowup-Rizz-Development/team-standards/blob/main/docs/service-setup.md#7-erp-mcp), 커밋과 PR 형식은 [일하는 방식: 커밋과 PR](https://github.com/Glowup-Rizz-Official/dev-agent/blob/main/docs/%EC%BB%A4%EB%B0%8B%EA%B3%BC-PR.md)이다. 이 파일에 규칙 원문을 복사하지 않는다.
