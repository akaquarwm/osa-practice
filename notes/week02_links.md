# 2주차 실습 링크와 기록

## 1교시

- 저장소: https://github.com/akaquarwm/osa-practice
- 충돌 해결 merge commit: f634df8
- 상세 기록: week02_merge.md

## 2교시 — 교수님 허용에 따른 개인 실습

- Issue: https://github.com/akaquarwm/osa-practice/issues/1
- PR: https://github.com/akaquarwm/osa-practice/pull/2
- base: akaquarwm/osa-practice의 main
- compare: 같은 저장소의 feature/contributing
- 결과: PR #2가 Merged이고 Closes #1에 연결된 Issue #1이 completed로 닫힌 것을 확인했다.
- 병합 commit: 2c3420a
- Fork: 개인 실습이므로 생략.
- 타인 리뷰 코멘트 URL: 해당 없음(상호 리뷰 생략).
- Request changes 및 Approve: 수행하지 않음. 타인 리뷰를 받은 것으로 기록하지 않는다.
- 자체 점검: README 기여 방법, 브랜치 이름 예시, 변경 범위, 비밀정보 미포함을 확인했다.
- 예상: PR에는 main 기준의 기여 방법 추가가 나타나고 Closes #1이 병합 시 Issue 종료와 연결될 것이다.
- 실제: 변경 파일 두 개와 2개 commit을 확인했고, 병합 후 Issue가 종료되었다.
- Fork는 다른 소유자의 저장소를 내 계정에서 수정할 공간을 만들고, branch는 한 저장소 안에서 작업 흐름을 분리한다.

## 병합 후 graph

```text
*   2c3420a Merge pull request #2 from akaquarwm/feature/contributing
|\
| * 7677e0a Record individual contribution exercise
| * 881aeba Add contributing section to README
|/
* f92f389 Add issue and PR templates
* fc52947 Record merge conflict exercise
*   f634df8 Merge branch feature/readme
|\
| * b1cceee Describe repository purpose
* | 85f09be State repository scope
|/
* e70c9b8 Add README
* 2d4a946 Add environment report
```
