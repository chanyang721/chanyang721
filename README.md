## Open Source Contributions

### [GitHub MCP Server](https://github.com/github/github-mcp-server) · Go

- PR 내용 리소스의 파일 경로 자동완성이 PR이 아닌 기본 브랜치의 파일 트리를 보여 주던 문제를 고쳤습니다. 이제 PR head 트리를 조회해 PR에서 추가한 파일이 제안되고, PR에서 지운 파일을 제안해 404가 나는 일이 없습니다. [#3860](https://github.com/github/github-mcp-server/pull/3860)

### [Herdr App](https://github.com/herdrdev/herdr-app) · Rust, TypeScript

- 모드를 반복해 다시 불러오면 창의 스크립트 VM(QuickJS) 메모리가 차서 창 전체가 `out of memory`로 멈추던 문제를 고쳤습니다. 힙 한도의 75%에 이르거나 리로드가 메모리 부족으로 실패하면 모드를 새 VM으로 옮깁니다. [#760](https://github.com/herdrdev/herdr-app/pull/760)
- 형식이 잘못된 대상 ID(`{"id":123}` 등)가 활성 탭으로 대체돼, 오류 대신 실행 중인 터미널을 닫던 문제를 고쳤습니다. 명령을 처리하기 전에 ID 형식을 검증합니다. [#297](https://github.com/herdrdev/herdr-app/pull/297)
- Windows 파일 패널에서 OneDrive 폴더가 파일로 표시되고, 둥근 따옴표(`O’Brien`)가 든 경로가 열리지 않던 문제를 고쳤습니다. [#354](https://github.com/herdrdev/herdr-app/pull/354)
- 찾기 결과가 한글·이모지 같은 넓은 문자로 끝나면 그 글자의 왼쪽 절반만 강조되던 문제를 고쳤습니다. [#587](https://github.com/herdrdev/herdr-app/pull/587)

### [Herdr Core](https://github.com/herdrdev/herdr-core) · Rust

- 프로그램을 잃고 재시작을 기다리는 부모 터미널에 메시지 전달을 쉬지 않고 재시도해 CPU 코어 하나를 100% 점유하던 문제를 고쳤습니다. [#124](https://github.com/herdrdev/herdr-core/pull/124)
- `hc wait --output`이 출력 청크 경계에서 잘린 UTF-8 문자를 깨뜨려 `준비 완료` 같은 문자열을 찾지 못하고 시간 초과되던 문제를 고쳤습니다. 아직 완성되지 않은 끝 바이트는 다음 청크와 함께 디코딩합니다. [#129](https://github.com/herdrdev/herdr-core/pull/129)
- `hc keep --off`가 이미 종료 처리된 터미널을 `live`로 응답하던 문제를 고쳤습니다. [#125](https://github.com/herdrdev/herdr-core/pull/125)

<!--
## Language
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E.svg?&style=for-the-badge&logo=JavaScript&logoColor=black)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6.svg?&style=for-the-badge&logo=TypeScript&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1.svg?&style=for-the-badge&logo=MySQL&logoColor=white)
![NodeJS](https://img.shields.io/badge/Node.js-43853D?style=for-the-badge&logo=node.js&logoColor=white)


## Framework
![NestJs](https://img.shields.io/badge/Nest.js-E0234E?style=for-the-badge&logo=nestjs&logoColor=#E0234E)
-->
