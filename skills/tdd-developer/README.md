# tdd-developer 스킬 사용법

이 폴더의 [tdd-developer.md](./tdd-developer.md)는 언어·프레임워크에 무관한 범용 TDD 개발 스킬입니다. `Claude`뿐 아니라 `ChatGPT`, `Gemini` 등 다른 AI 에이전트에서도 그대로 사용할 수 있습니다.

같은 내용이 Claude Code용으로는 [../../.claude/skills/tdd-developer/SKILL.md](../../.claude/skills/tdd-developer/SKILL.md)에도 있으며, Claude Code에서는 `/tdd-developer`로 바로 호출됩니다. 이 폴더의 버전은 다른 도구에 붙여넣기 위한 사본입니다. 스킬 내용을 수정할 때는 두 파일을 함께 갱신하세요.

## Claude Code

- 이미 `.claude/skills/tdd-developer/SKILL.md`에 있어 별도 설치 없이 이 저장소 안에서 자동 인식됩니다.
- 대화에서 "TDD로 개발해줘"라고 요청하거나, 관련 작업(신규 기능/버그 수정)을 시키면 자동으로 적용됩니다.

## ChatGPT

- **Custom GPT**: GPT 빌더의 "Instructions" 필드에 `tdd-developer.md` 전체 내용을 붙여넣습니다.
- **Projects/Custom Instructions**: 설정의 "Custom instructions" 또는 프로젝트 지침에 붙여넣으면 해당 대화/프로젝트 내내 적용됩니다.
- **단발성 사용**: 대화 맨 처음 메시지로 파일 내용을 붙여넣고 "이 지침에 따라 TDD로 개발해줘"라고 요청합니다.

## Gemini

- **Gems**: Gem 생성 시 "Instructions" 항목에 파일 내용을 붙여넣습니다.
- **일반 대화**: 대화 시작 시 지침을 붙여넣고 이어서 요구사항을 전달합니다.

## 기타 에이전트 (Cursor, Copilot Chat 등)

- 대부분 프로젝트 규칙 파일(예: `.cursorrules`, `AGENTS.md` 등)에 이 문서 내용을 포함시키면 됩니다.
- 코드 실행 도구가 없는 환경이면 문서의 "에이전트 환경별 적용 가이드" 절을 참고해, 사이클마다 사용자에게 테스트 실행 결과를 확인받는 방식으로 진행합니다.
