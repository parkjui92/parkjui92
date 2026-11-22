# 박주이 · Jui Park

데이터와 AI로 과학기술정책을 연구합니다. 한양대학교 과학기술정책연구소와 정책한걸음에서 활동하고 있습니다. 연구하며 만든 Claude Code 도구를 이곳에 공개합니다.

*I research science and technology policy with data and AI, working with the Science and Technology Policy Institute at Hanyang University and 정책한걸음 (The Step in Public Policy). This is where I share the Claude Code tools I built along the way.*

<img src="assets/flow.png" width="100%" alt="연구 단계마다 쓰는 도구. 자료 찾기(prism-db, korea-cabinet-stp, awesome-research-stages) → 설계 검토 → 집필(policy-research-kit, socsci-paper-kit, report-to-brief) → 초안 검수 → 검증·교정(fact-verify, paper-proofread, report-rules) → 양식·그림(form-tailor, doc-figure) → 공유·강의(deident, lecture-deck-kit)">

## 멀티에이전트 하네스

역할을 나눈 서브에이전트가 설계 검토와 초안 검수 게이트를 통과해야 다음 단계로 넘어가는 Claude Code 플러그인입니다.

| 저장소 | 만드는 것 |
|---|---|
| [policy-research-kit](https://github.com/parkjui92/policy-research-kit) | 정책연구보고서·정책브리프 (.hwpx) |
| [socsci-paper-kit](https://github.com/parkjui92/socsci-paper-kit) | 사회과학 논문, 심사의견 대응 (.docx) |
| rnd-proposal-kit (비공개) | 정부 R&D 제안서 초안 (.hwpx) |

## 에이전트 스킬

| 저장소 | 하는 일 |
|---|---|
| [fact-verify](https://github.com/parkjui92/fact-verify) | 출처가 진짜인지 확인, 발췌를 원문과 기계 대조 |
| [paper-proofread](https://github.com/parkjui92/paper-proofread) | 한국어 원고 교정교열 (논문·보고서·공문서), 한글 파일은 원본에 바로 반영 |
| [report-rules](https://github.com/parkjui92/report-rules) | 보고서 작성 규칙과 초안 점검기 |
| [report-to-brief](https://github.com/parkjui92/report-to-brief) | 긴 보고서를 1~8쪽 브리프로 압축 |
| [form-tailor](https://github.com/parkjui92/form-tailor) | 기관 양식 샘플대로 새 문서 작성 |
| [doc-figure](https://github.com/parkjui92/doc-figure) | 문서용 삽도, 한글이 깨지지 않는 코드 렌더 |
| [lecture-deck-kit](https://github.com/parkjui92/lecture-deck-kit) | HTML 강의자료, 브라우저에서 드래그해 바로 수정 |
| [rnd-eval-skills](https://github.com/parkjui92/rnd-eval-skills) | 정부 R&D 사업 평가 — 사업 논리·성과지표·예산 추이·유사중복·성과 주장 점검, 평가보고서 골격 |

## 도구와 데이터

| 저장소 | 하는 일 |
|---|---|
| [deident](https://github.com/parkjui92/deident) | 문서 민감정보 비식별화, 전 과정 로컬 |
| [prism-db](https://github.com/parkjui92/prism-db) | 정책연구용역(PRISM) 로컬 검색 CLI |
| [korea-cabinet-stp](https://github.com/parkjui92/korea-cabinet-stp) | 국무회의 안건 아카이브 (2018~2026) |
| [awesome-research-stages](https://github.com/parkjui92/awesome-research-stages) | 연구 단계별 오픈소스 도구 목록 |
| [deep-research-kit](https://github.com/parkjui92/deep-research-kit) | 여러 논문을 질문에 맞는 비교표로, 값마다 원문 문장으로 확인 |
| [kr-sti-data](https://github.com/parkjui92/kr-sti-data) | 과학기술·R&D 통계 수집기 (KOSIS·NABOSTATS·NTIS) |
| [kr-grant-trace](https://github.com/parkjui92/kr-grant-trace) | 정부 R&D 과제번호로 사사 논문 추적 |
| [rnd-program-logic](https://github.com/parkjui92/rnd-program-logic) | 정부 R&D 사업 논리모형·성과지표 설계 점검기 |
| [policy-did](https://github.com/parkjui92/policy-did) | 정책평가 인과추론 작업대, 추정 전에 설계서와 식별 가정 점검 |
| [won-diff](https://github.com/parkjui92/won-diff) | 예산표 단위 맞춤과 금액 변경 검토 |

## 처음이라면

가장 가벼운 것은 paper-proofread입니다.

```bash
mkdir -p ~/.claude/skills && cd ~/.claude/skills && git clone https://github.com/parkjui92/paper-proofread.git
```

Claude Code를 다시 켜고 "이 문단 교정해줘"라고 하면 됩니다. 막힌 곳이 있으면 그 저장소의 Issues에 남겨 주세요.

## 알아두실 점

- 모두 초안과 점검 결과를 만드는 도구입니다. 내보내기 전 판단은 사람이 합니다.
- 코드는 대부분 MIT입니다. 수집 데이터(prism-db·korea-cabinet-stp)는 원 자료의 이용 조건(공공누리)을 따릅니다. 자세한 조건은 각 저장소의 LICENSE에 있습니다.
- 질문과 버그는 각 저장소의 Issues로 받습니다.

<details>
<summary>English</summary>

- **Multi-agent harnesses** — [policy-research-kit](https://github.com/parkjui92/policy-research-kit) (policy reports and briefs), [socsci-paper-kit](https://github.com/parkjui92/socsci-paper-kit) (social science papers and reviewer responses). Role-split subagents must pass a design review and a draft review before moving on.
- **Agent skills** — [fact-verify](https://github.com/parkjui92/fact-verify) (source verification with a claim–evidence ledger), [paper-proofread](https://github.com/parkjui92/paper-proofread) (Korean proofreading for papers, reports and government documents, with in-place .hwpx revisions), [report-rules](https://github.com/parkjui92/report-rules), [report-to-brief](https://github.com/parkjui92/report-to-brief), [form-tailor](https://github.com/parkjui92/form-tailor), [doc-figure](https://github.com/parkjui92/doc-figure), [lecture-deck-kit](https://github.com/parkjui92/lecture-deck-kit), [rnd-eval-skills](https://github.com/parkjui92/rnd-eval-skills) (Korean government R&D program evaluation checks)
- **CLI and data** — [deident](https://github.com/parkjui92/deident) (local de-identification of Korean documents), [prism-db](https://github.com/parkjui92/prism-db), [korea-cabinet-stp](https://github.com/parkjui92/korea-cabinet-stp), [awesome-research-stages](https://github.com/parkjui92/awesome-research-stages), [deep-research-kit](https://github.com/parkjui92/deep-research-kit) (literature comparison tables checked against source sentences), [kr-sti-data](https://github.com/parkjui92/kr-sti-data) (Korean S&T statistics collector), [kr-grant-trace](https://github.com/parkjui92/kr-grant-trace) (grant numbers to publications), [rnd-program-logic](https://github.com/parkjui92/rnd-program-logic) (logic-model and indicator design checker), [policy-did](https://github.com/parkjui92/policy-did) (design and identification checks before causal estimates), [won-diff](https://github.com/parkjui92/won-diff) (budget table comparison)

Questions and bug reports go to each repository's Issues.

</details>

## 연락

parkjui92@gmail.com
