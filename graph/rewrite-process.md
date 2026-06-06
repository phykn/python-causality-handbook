# Rewrite Process

한국어 작업은 번역이 아니라 강의노트화다.

원문 문장 순서를 보존하려고 하지 않는다. 원문이 가진 evidence, 코드, 그림, 수식, 식별 논리는 보존하되, 한국어 독자가 판단을 따라갈 수 있는 순서로 설명을 다시 짠다.

대상 독자는 중/고등학생이다. 어려운 내용을 빼는 것이 아니라, 어려운 내용이 필요한 이유를 먼저 보여주고 그 다음에 용어, 수식, 코드를 붙인다.

## Unit Of Work

한 번에 처리하는 단위는 `one chapter plus its graph node`다.

예:

- source: `causal-inference-for-the-brave-and-true/11-Propensity-Score.ipynb`
- target: `causal-inference-for-the-brave-and-true-ko/11-Propensity-Score.ipynb` after recreating the Korean folder
- graph node: [design-without-randomization](nodes/design-without-randomization.md)
- audience rule: [audience](audience.md)
- explanation gaps: [explanation-gaps](explanation-gaps.md)

## Procedure

1. `coverage`에서 장이 속한 node를 확인한다.
2. [audience](audience.md)의 `Explanation Ladder`를 확인한다.
3. node의 `Question`을 장 첫머리의 한국어 문제 제기로 바꾼다.
4. node의 `Student Bridge`와 [explanation-gaps](explanation-gaps.md)에서 선행 설명이 필요한 용어를 고른다.
5. 원문의 heading을 그대로 번역하지 말고 `reader state`가 바뀌는 지점으로 재배열한다.
6. 코드 셀은 가능한 유지한다. 단, 코드가 설명의 흐름을 끊으면 먼저 직관을 쓰고 코드를 evidence로 배치한다.
7. 수식은 생략하지 않는다. 수식 앞에는 "왜 이 식이 필요한가"를 먼저 설명한다.
8. 그림과 예시는 원문의 증거로 남긴다. 한국어 설명은 그림을 보는 순서를 안내한다.
9. 장 끝에는 다음 node로 넘어가는 질문과 학생용 확인 질문을 쓴다.

## Chapter Template

각 장은 다음 구조를 기본으로 한다.

```text
1. 이 장의 질문
2. 생활 속 예시
3. 왜 단순한 비교가 실패하는가
4. 공정한 비교를 만들기 위해 필요한 조건
5. 방법 이름과 핵심 용어
6. estimator가 하는 일
7. 코드, 그림, 수식
8. 한계와 오해하기 쉬운 지점
9. 학생용 확인 질문
10. 다음 장으로 넘어가는 질문
```

## Rewrite Rules

- 기법 이름보다 판단 문제를 먼저 둔다.
- 중/고등학생이 이미 아는 생활 상황에서 시작한다.
- 새 용어는 상황, 질문, 실패한 쉬운 비교 뒤에 붙인다.
- 원문 jokes나 memes는 의미를 해치지 않으면 유지하되, 한국어 이해를 방해하면 설명 뒤로 보낸다.
- "이 방법은 좋다"보다 "이 방법은 어떤 실패를 막고, 어떤 실패는 못 막는가"를 쓴다.
- `ATE`, `CATE`, `confounding`, `selection`, `identification`, `nuisance` 같은 용어는 처음 등장할 때 영어와 한국어 설명을 같이 둔다.
- 영어 약어는 첫 등장 때 풀어 쓰고, 그 장 안에서는 같은 표현을 유지한다.
- 새 비유를 추가할 수 있지만, 코드와 수식이 보여주는 사실을 흐리면 제거한다.

## Student Checkpoint

각 큰 절 끝에는 짧은 확인 질문을 하나 둔다.

좋은 질문:

- `학원을 다닌 학생과 다니지 않은 학생의 평균 점수만 비교하면 왜 위험할까?`
- `이 방법은 어떤 비교를 더 공정하게 만들고, 어떤 문제는 아직 남기는가?`

나쁜 질문:

- `propensity score의 정의를 쓰시오.`
- `DID estimator 공식을 암기하시오.`

## Review Gate

한 장을 완료했다고 말하려면 다음을 확인한다.

- 원본의 핵심 주장, 코드, 그림, 수식이 빠지지 않았다.
- 한국어 장 첫머리가 실제 질문으로 시작한다.
- 첫 예시는 중/고등학생이 이해할 수 있는 생활 상황이다.
- 새 용어가 나오기 전에 그 용어가 필요한 비교 문제가 보인다.
- 독자가 다음에 무엇을 판단해야 하는지 보인다.
- 학생용 확인 질문이 장 안에 있다.
- 해당 graph node의 `Rewrite Focus`가 반영되어 있다.
- 원본 폴더는 변경하지 않았다.
