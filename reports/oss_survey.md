# 공개 AI 프로젝트 탐색표 — 1주차

- 작성자 표시 이름: student01
- 조사일: 2026-10-29 (한국 시간)
- 조사 기준: 공식 GitHub 파일 및 API. 열린 이슈는 PR을 제외한 수이며 이후 달라질 수 있다.
- 조사 대상: `ollama/ollama`, `huggingface/transformers`, `vllm-project/vllm`

## 탐색표

| 저장소 | 라이선스(SPDX ID) | 최근 커밋(며칠 전) | 열린 이슈 수 | 기여 가이드 | 릴리스 주기 |
|---|---|---|---|---|---|
| `ollama/ollama` | MIT | 0일 전 (10월 29일 12:46 KST) | 2612 | 있음 — Set up | 최근 3개 기준 약 2~3일 |
| `huggingface/transformers` | Apache-2.0 | 0일 전 (10월 29일 08:25 KST) | 378 | 있음 — Contents | 최근 3개 기준 약 3~7일 |
| `vllm-project/vllm` | Apache-2.0 | 0일 전 (10월 29일 15:30 KST) | 2721 | 있음 — Job Board (docs/contributing/README.md) | 최근 3개 기준 약 13일 |

최근 커밋 시점은 자동 조사 시점의 기본 브랜치 기준으로 갱신했다. 릴리스 주기는 아래 세 발표 사이의 간격을 반올림한 값이며 고정 일정은 아니다.

## 근거 URL

| 저장소 | 라이선스 | 커밋 | 이슈 | 기여 가이드 | 릴리스 |
|---|---|---|---|---|---|
| `ollama/ollama` | https://github.com/ollama/ollama/blob/main/LICENSE | https://api.github.com/repos/ollama/ollama/commits?per_page=1 | https://api.github.com/search/issues?q=repo:ollama/ollama+is:issue+is:open&per_page=1 | https://github.com/ollama/ollama/blob/main/CONTRIBUTING.md | https://github.com/ollama/ollama/releases |
| `huggingface/transformers` | https://github.com/huggingface/transformers/blob/main/LICENSE | https://api.github.com/repos/huggingface/transformers/commits?per_page=1 | https://api.github.com/search/issues?q=repo:huggingface/transformers+is:issue+is:open&per_page=1 | https://github.com/huggingface/transformers/blob/main/CONTRIBUTING.md | https://github.com/huggingface/transformers/releases |
| `vllm-project/vllm` | https://github.com/vllm-project/vllm/blob/main/LICENSE | https://api.github.com/repos/vllm-project/vllm/commits?per_page=1 | https://api.github.com/search/issues?q=repo:vllm-project/vllm+is:issue+is:open&per_page=1 | https://github.com/vllm-project/vllm/blob/main/docs/contributing/README.md | https://github.com/vllm-project/vllm/releases |

## 최근 릴리스 근거 (한국 날짜)

| 저장소 | 최근 발표 3개 | 간격 |
|---|---|---|
| Ollama | v0.40.13 (10/29), v0.40.12 (10/27), v0.40.11 (10/24) | 약 2일, 3일 |
| Transformers | v5.21 (10/27), v5.20.2 (10/20), v5.20.1 (10/16) | 약 7일, 3일 (시간 차이 반올림) |
| vLLM | v0.32.0 (10/18), v0.31.0 (10/05), v0.30.0 (09/22) | 약 13일, 13일 |

## 오픈소스 AI 정의(OSAID) 판정

OSAID의 세 공개 항목은 데이터 정보·코드·파라미터다. 아래는 소프트웨어의 공개 코드를 이 항목에 대응시킨 수업용 판정이며, 개별 AI 시스템 전체의 OSAID 충족을 인증하는 것은 아니다.

1. `ollama/ollama`: 이 프로젝트는 실행 도구의 소스 코드가 MIT로 공개되어 OSAID의 코드 항목에 대응하며, 학습 데이터 정보와 파라미터 공개 여부는 개별 모델에서 확인해야 한다.
2. `huggingface/transformers`: 이 프로젝트는 모델 활용 라이브러리의 코드가 Apache-2.0으로 공개되어 코드 항목에 대응하며, 데이터 정보와 파라미터 항목은 개별 모델의 문제다.
3. `vllm-project/vllm`: 이 프로젝트는 추론·서빙 코드가 Apache-2.0으로 공개되어 코드 항목에 대응하며, 데이터 정보와 파라미터 항목은 실행할 모델마다 별도로 확인해야 한다.

공개된 도구 코드만으로 특정 모델의 전체 학습 코드·데이터 정보·파라미터가 모두 공개되었다고 판단할 수 없다.
정의 근거: https://opensource.org/ai/open-source-ai-definition

## 도구와 모델의 라이선스

Ollama 도구는 MIT이고 그 도구로 실행하는 `qwen3:8b` 모델의 license 파일은 Apache-2.0이므로 둘은 다르며, 도구의 라이선스만 보고 모델의 사용 조건을 판단하면 안 된다.

- 도구 근거: https://github.com/ollama/ollama/blob/main/LICENSE
- 크기 태그 페이지: https://ollama.com/library/qwen3:8b
- 모델 license 원문: https://ollama.com/library/qwen3:8b/blobs/d18a5cc71b84

## 살아 있는 프로젝트의 근거

활동 지표 2개:

1. 최근 커밋: 세 프로젝트 모두 조사일인 2026-10-29 한국 날짜에 기본 브랜치 수정이 확인되어 코드 관리가 이어지고 있다고 판단한다. 근거는 위 커밋 URL이다.
2. 최근 릴리스: Ollama는 약 2~3일, Transformers는 약 3~7일, vLLM은 약 13일 간격으로 최근 버전 3개가 발표되어 배포 활동이 이어지고 있다. 근거는 위 릴리스 URL이다.

열린 이슈 수가 많다는 사실만으로 활발하다거나 품질이 낮다고 단정하지 않는다.

## 조사 전 예상

세 프로그램을 처음 접해서 사용 조건은 아직 모르겠다. 최근에도 개발되고 있을 것 같으며, 실제 저장소에서 확인해 보겠다.
