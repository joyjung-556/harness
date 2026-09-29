# R4 — 산출물과 재개 방식

아래 파일은 하네스 실행 시 생성할 산출물의 이름이다.

| 단계 | 산출물 |
|---|---|
| ① 레퍼런스 수집·분석 | `reference-analysis.md` |
| ② 화면 설계 | `screen-spec.md` |
| ③ 키스크린 제작·승인 | `key-screens.md` — Figma 링크, 각 화면의 390×844 크기, 승인 결과 기록 |
| ④ 디자인 제작 | `design-tokens.json`, `components.md`, `screens.md` |
| ⑤ 가이드 검토 | `design-review.json` |

판정 규칙의 단일 기준 파일은 `harness-rules.json`이다. 검사 가능한 각 규칙에 PRD 또는 디자인 가이드의 출처를 함께 기록한다. PRD와 디자인 가이드의 원문은 별도로 유지한다.

각 실행의 산출물은 `runs/YYYYMMDD-HHmmss/` 형식의 별도 폴더에 저장한다. 같은 폴더의 `run-state.json`에 단계별 산출물과 게이트 결과를 기록한다. 중단되면 마지막으로 통과한 게이트 다음 단계부터 재개한다.
