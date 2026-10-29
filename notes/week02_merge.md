# 2주차 1교시 — 원격 연결과 충돌 해결

- 저장소: https://github.com/akaquarwm/osa-practice
- 실습일: 2026-10-29
- 실행 전 예상(자동 실습 계획): main과 feature/readme가 같은 줄을 다르게 수정하면 merge 충돌이 발생할 것이다.
- 실제: git merge feature/readme 실행 시 CONFLICT (content)와 UU README.md가 나타났다.
- 경계 경로: git merge --abort 후 작업 폴더가 clean으로 복원됨을 확인하고 다시 merge하여 같은 충돌을 재현했다.
- 해결: 충돌 마커 세 종류를 제거하고 두 문장의 의도를 하나로 합쳐 merge commit을 만들었다.
- 최종 문장: 이 저장소는 오픈소스 AI 응용 수업의 실습 기록이며 로컬 AI 도우미 프로젝트의 시작점이다.
- 설명: 충돌은 두 수정 중 어떤 내용을 남길지 사람의 결정을 요청하는 상태다.
- 권한 없는 타인 저장소에 push하는 실패 실험은 실행하지 않았다.

## 병합 직후 이력

*   f634df8 Merge branch 'feature/readme'
|\  
| * b1cceee Describe repository purpose
* | 85f09be State repository scope
|/  
* e70c9b8 Add README
* 2d4a946 Add environment report