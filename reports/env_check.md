# 실습환경 점검표 — 1주차

- 작성자 표시 이름: akaquarwm
- PC 구분:  개인 노트북 
- 점검 방법: 새 PowerShell 창에서 `env_check.ps1` 실행 후 실패 항목은 수동 명령으로 재확인

## 도구

| 도구 | 확인 명령 | 버전 문자열(첫 줄 그대로) | 상태 | 조치(실패 시) |
|---|---|---|---|---|
| Git | `git --version` | git version 2.56.0.windows.2 | 정상 | 없음 |
| VS Code | `code --version` | 1.143.1 | 정상 | 없음 |
| uv | `uv --version` | uv 0.13.1 (62faed335 2026-10-13 x86_64-pc-windows-msvc) | 정상 | 없음 |
| Ollama | `ollama --version` | 명령을 찾을 수 없음 | 실패 | 미설치 → 4주차 전까지 설치 |
| NVIDIA 드라이버 | `nvidia-smi` | 명령을 찾을 수 없음 | 실패 | CPU + 소형 모델 경로로 진행 |

- `uv` 설치 경로(`Get-Command uv | Select-Object -ExpandProperty Source`): %USERPROFILE%\.local\bin\uv.exe
- Ollama 행이 `실패`이고 `명령을 찾을 수 없음`이면 **미설치**다. 이번 주에는 설치하지 않고 조치 칸에 "미설치 → 4주차 전까지 설치"라고 적는다.
- Ollama 행에 `Warning: client version is …`가 들어갔다면 **설치는 됐고 서버만 꺼진 것**이다. 조치 칸에 "서버 꺼짐"이라고 적는다.

## GPU

| 항목 | 값 |
|---|---|
| GPU 이름 | 없음 |
| VRAM(MiB) | 해당 없음 |
| 드라이버 버전 | 해당 없음 |
| GPU가 없을 때 대체 경로 | CPU + 소형 모델(`qwen3:0.6b`) |

## 계정 (비밀번호·토큰·이메일 기록 금지)

| 서비스 | 표시 이름 | 로그인 확인 | 공개 프로필의 불필요한 개인정보 |
|---|---|---|---|
| GitHub | akaquarwm | 확인함 | 없음 |
| Hugging Face | aquarwm | 확인함 | 없음 |

## 실패 항목과 조치

1. Ollama — 미설치 → 4주차 전까지 설치 예정.
2. NVIDIA — GPU 없음 → CPU + 소형 모델 경로로 진행.

## 4주차 전까지 할 일 (개인 노트북)

실습실 PC를 쓰면 조교가 이미 준비했으므로 "해당 없음"으로 둔다.

| 항목 | 상태 | 완료 날짜 |
|---|---|---|
| Ollama 설치 — 새 창에서 `ollama --version`이 버전 문자열 출력 | 미완 |  |
| 강의자가 공지한 모델 — `ollama list`에 보임 | 미완 |  |

## 한 문장 결론

이 PC는 CPU + 소형 모델 경로로 실습을 진행하며, 4주차 전까지 Ollama와 강의자가 공지한 모델을 준비한다.