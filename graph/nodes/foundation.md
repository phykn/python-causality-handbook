# Foundation

## Question

예측 질문과 인과 질문은 왜 다른가?

## Reader State

독자는 데이터 분석이 보통 `Y를 잘 예측하는 모델`로 끝난다고 생각한다. 이 노드는 그 생각을 `X를 바꾸면 Y가 어떻게 달라지는가`라는 질문으로 전환한다.

## Core Idea

인과추론은 반사실 비교를 다룬다. 같은 사람이나 단위가 treatment를 받은 세계와 받지 않은 세계를 동시에 관측할 수 없기 때문에, 믿을 만한 대체 비교를 만들어야 한다.

무작위 실험은 그 비교를 가장 직접적으로 만든다. 통계 리뷰는 그 비교 결과가 얼마나 흔들릴 수 있는지 보여준다.

## Student Bridge

학생에게는 `반사실`을 먼저 말하지 않는다. 먼저 "같은 학생이 학원을 다닌 경우와 다니지 않은 경우를 동시에 볼 수 없다"고 말한다.

추가 설명이 필요한 부분:

- treatment: 우리가 바꾸고 싶은 선택이나 행동.
- outcome: 그 선택 뒤에 보고 싶은 결과.
- counterfactual: 실제로 선택하지 않은 쪽의 결과.
- random assignment: 두 집단을 비슷하게 만들기 위해 운에 맡기는 배정.
- standard error: 같은 비교를 여러 번 하면 결과가 흔들리는 정도.

## Source Chapters

- 01 Introduction To Causality
- 02 Randomised Experiments
- 03 Stats Review

## Edges

- Previous: [core](../core.md)
- Next: [causal-graphs](causal-graphs.md)
- Cross-link: [inference](inference.md)

## Rewrite Focus

한국어 장은 `상관관계가 충분한가`라는 질문에서 시작한다.

설명 순서:

1. prediction과 causal question을 비교한다.
2. potential outcome을 "동시에 볼 수 없는 두 결과"로 설명한다.
3. random assignment가 왜 두 집단을 비교 가능하게 만드는지 보인다.
4. estimate는 숫자 하나가 아니라 uncertainty를 가진 판단이라는 점으로 마무리한다.

## Common Failure

이 노드를 단순히 "인과추론 개론, 실험, 통계 복습"으로 쓰면 안 된다. 세 장은 하나의 질문을 만든다: `어떤 비교를 믿을 수 있는가`.
