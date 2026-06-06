# Heterogeneity

## Question

평균 효과가 아니라 사람마다 다른 효과가 필요하면 무엇을 추정해야 하는가?

## Reader State

독자는 ATE를 추정할 수 있지만, 실제 정책에서는 누구에게 treatment를 줄지 결정해야 한다.

## Core Idea

CATE는 covariate가 주어졌을 때 treatment effect가 어떻게 달라지는지 나타내는 함수다.

plug-and-play estimator, target transformation, meta learner는 flexible prediction model을 사용해 heterogeneous treatment effect를 추정하려는 방법이다.

## Student Bridge

학생에게는 ATE와 CATE를 먼저 숫자 예시로 나눈다. 평균으로는 도움이 필요한 학생을 찾을 수 없다는 점을 보여준다.

추가 설명이 필요한 부분:

- ATE: 전체를 평균냈을 때의 효과.
- CATE: 비슷한 특성을 가진 사람들에게서의 효과.
- heterogeneity: 효과가 사람마다 다르게 나타나는 현상.
- target transformation: 알고 싶은 효과를 모델이 배울 수 있는 숫자로 바꾸는 일.
- meta learner: 기존 예측 모델을 조합해 효과를 추정하는 방식.

## Source Chapters

- 18 Heterogeneous Treatment Effects and Personalization
- 19 Evaluating Causal Models
- 20 Plug-and-Play Estimators
- 21 Meta Learners
- 23 Challenges with Effect Heterogeneity and Nonlinearity

## Edges

- Previous: [prediction-policy](prediction-policy.md)
- Next: [orthogonal-ml](orthogonal-ml.md)
- Cross-link: [inference](inference.md)

## Rewrite Focus

한국어 설명은 personalization을 "더 정교한 예측"으로 축소하지 않는다.

설명 순서:

1. ATE가 policy targeting에 부족한 이유를 보인다.
2. CATE를 `개인 특성별 효과 함수`로 설명한다.
3. target transformation과 meta learner가 ML 문제로 바꾸는 방식을 설명한다.
4. S, T, X learner를 데이터 상황별 선택으로 정리한다.
5. heterogeneity와 nonlinearity가 effect 해석을 어렵게 하는 지점을 남긴다.

## Common Failure

CATE를 outcome prediction처럼 설명하면 안 된다. CATE는 `결과값`이 아니라 `처치했을 때의 변화량`이다.
