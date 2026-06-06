# Route

이 그래프의 기본 route는 원문 장 순서를 그대로 보존하되, 한국어 설명은 판단 질문 단위로 묶는다.

## Phase 1: Ask The Right Question

Node: [foundation](nodes/foundation.md)

Source chapters:

- 01 Introduction To Causality
- 02 Randomised Experiments
- 03 Stats Review

Reader should learn:

- 인과 질문은 예측 질문과 다르다.
- 무작위 실험은 비교 가능성을 보장하는 benchmark다.
- estimate는 항상 uncertainty를 가진다.

Next question:

- `무작위 실험이 없을 때 어떤 비교가 망가지는가?`

## Phase 2: See What Breaks The Comparison

Nodes:

- [causal-graphs](nodes/causal-graphs.md)
- [regression-adjustment](nodes/regression-adjustment.md)

Source chapters:

- 04 Graphical Causal Models
- 05 Linear Regression
- 06 Grouped and Dummy Regression
- 07 Beyond Confounders

Reader should learn:

- confounding과 selection은 서로 다른 실패다.
- control은 많이 넣을수록 좋은 것이 아니다.
- regression은 조건부 평균 비교를 구현하는 도구다.

Next question:

- `관측 변수 조정만으로 부족하면 어떤 설계가 비교를 대신 만들어주는가?`

## Phase 3: Build A Design Without Randomization

Nodes:

- [design-without-randomization](nodes/design-without-randomization.md)
- [panel-time](nodes/panel-time.md)

Source chapters:

- 08 Instrumental Variables
- 09 Non Compliance and LATE
- 10 Matching
- 11 Propensity Score
- 12 Doubly Robust Estimation
- 13 Difference-in-Differences
- 14 Panel Data and Fixed Effects
- 15 Synthetic Control
- 16 Regression Discontinuity Design

Reader should learn:

- IV는 treatment가 아니라 treatment를 움직이는 external variation을 쓴다.
- LATE는 누구의 효과를 추정하는지 좁힌다.
- matching, propensity score, doubly robust는 관측 변수 기반 비교를 다르게 구성한다.
- DID, fixed effects, synthetic control, RDD는 시간, 단위, 절단점을 이용해 비교를 만든다.

Next question:

- `평균 효과가 아니라 사람마다 다른 효과가 필요하면 무엇이 달라지는가?`

## Phase 4: Turn Causal Estimates Into Policy Inputs

Nodes:

- [prediction-policy](nodes/prediction-policy.md)
- [heterogeneity](nodes/heterogeneity.md)
- [inference](nodes/inference.md)

Source chapters:

- 17 Predictive Models 101
- 18 Heterogeneous Treatment Effects and Personalization
- 19 Evaluating Causal Models
- 20 Plug-and-Play Estimators
- 21 Meta Learners
- When Prediction Fails
- Prediction Metrics For Causal Models

Reader should learn:

- 예측 모델은 정책 입력이 될 수 있지만, 예측 성능이 인과 성능을 보장하지 않는다.
- CATE는 누구에게 처치할지 결정하기 위한 효과 함수다.
- causal model 평가는 prediction metric이 아니라 정책 이득과 효과 ranking을 봐야 한다.

Next question:

- `flexible ML을 쓰면서도 인과 estimate의 bias를 어떻게 줄일까?`

## Phase 5: Use Flexible Models Without Losing Identification

Nodes:

- [orthogonal-ml](nodes/orthogonal-ml.md)
- [modern-did-sdid](nodes/modern-did-sdid.md)
- [inference](nodes/inference.md)

Source chapters:

- 22 Debiased Orthogonal Machine Learning
- 23 Challenges with Effect Heterogeneity and Nonlinearity
- 24 Difference-in-Differences Saga
- 25 Synthetic Difference-in-Differences
- Debiasing with Orthogonalization
- Debiasing with Propensity Score
- Conformal Inference for Synthetic Controls

Reader should learn:

- ML은 nuisance function 추정에 강하지만, treatment effect 추정에는 bias를 만들 수 있다.
- orthogonalization은 nuisance error가 target estimate에 직접 들어오지 않게 만든다.
- heterogeneous treatment effects는 DID와 nonlinear outcome에서도 기존 직관을 깨뜨린다.
- SDID와 conformal inference는 synthetic control 계열의 설계와 uncertainty를 확장한다.

Next question:

- `이 장을 한국어 강의노트로 만들 때 어떤 판단 순서를 먼저 보여줄 것인가?`

Go to [rewrite-process](rewrite-process.md).
