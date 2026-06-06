# Regression Adjustment

## Question

관측 변수로 비교를 맞출 수 있다면 회귀는 무엇을 해주는가?

## Reader State

독자는 회귀를 prediction model로 알고 있다. 이 노드는 회귀를 `조건이 같은 단위끼리 비교하는 장치`로 다시 읽게 한다.

## Core Idea

linear regression은 여러 covariate를 고정한 상태에서 treatment와 outcome의 평균 차이를 추정한다.

grouped data와 dummy regression은 회귀가 실제로 group 평균 비교를 일반화한다는 점을 보여준다.

## Student Bridge

학생에게는 regression을 "선을 긋는 방법"보다 "비슷한 조건끼리 비교하는 계산표"로 먼저 설명한다.

추가 설명이 필요한 부분:

- covariate: 비교를 공정하게 만들기 위해 같이 봐야 하는 조건.
- coefficient: 한 조건이 바뀔 때 결과가 얼마나 달라지는지 요약한 숫자.
- dummy variable: 집단 이름을 0과 1로 바꾼 표시.
- residual: 모델이 설명하고도 남은 차이.
- omitted variable bias: 중요한 조건을 빼먹어서 생기는 잘못된 비교.

## Source Chapters

- 05 The Unreasonable Effectiveness of Linear Regression
- 06 Grouped and Dummy Regression

## Edges

- Previous: [causal-graphs](causal-graphs.md)
- Next: [design-without-randomization](design-without-randomization.md)
- Cross-link: [orthogonal-ml](orthogonal-ml.md)

## Rewrite Focus

한국어 장에서는 `회귀 계수 = 기계적으로 나온 숫자`라는 인상을 피한다.

설명 순서:

1. 단순 평균 차이가 왜 confounding에 약한지 보인다.
2. 같은 covariate 값을 가진 사람끼리 비교한다는 직관을 준다.
3. regression coefficient가 그 조건부 비교를 요약한다는 점을 보인다.
4. dummy variable은 group별 intercept를 허용하는 방식으로 설명한다.
5. 회귀가 identification을 대신하지 않는다는 한계를 남긴다.

## Common Failure

회귀를 "모델 성능"으로 설명하면 책의 중심이 prediction으로 돌아간다. 여기서 회귀는 adjustment tool이다.
