# Coverage

이 문서는 원본 전체와 앞으로 만들 한국어 강의노트 범위를 그래프 노드에 연결한다.

`Source status`는 `causal-inference-for-the-brave-and-true/` 기준이다.
`Korean target`은 앞으로 다시 만들 `causal-inference-for-the-brave-and-true-ko/` 기준이다. 현재 한국어 노트북 폴더는 삭제된 상태이므로 모든 본문 장은 `not created`로 표시한다.

| Source | Korean target | Graph node | Rewrite angle |
| --- | --- | --- | --- |
| 01 Introduction To Causality | not created | [foundation](nodes/foundation.md) | 예측 질문과 인과 질문을 분리한다. |
| 02 Randomised Experiments | not created | [foundation](nodes/foundation.md) | 무작위 배정을 ideal comparison으로 설명한다. |
| 03 Stats Review | not created | [foundation](nodes/foundation.md), [inference](nodes/inference.md) | estimate에는 표준오차와 검정의 불확실성이 붙는다. |
| 04 Graphical Causal Models | not created | [causal-graphs](nodes/causal-graphs.md) | 그래프를 bias diagnosis 도구로 쓴다. |
| 05 Linear Regression | not created | [regression-adjustment](nodes/regression-adjustment.md) | 회귀를 조건부 비교로 읽는다. |
| 06 Grouped and Dummy Regression | not created | [regression-adjustment](nodes/regression-adjustment.md) | group 평균과 dummy 변수로 비교 구조를 보이게 한다. |
| 07 Beyond Confounders | not created | [causal-graphs](nodes/causal-graphs.md) | good control, bad control, selection을 구분한다. |
| 08 Instrumental Variables | not created | [design-without-randomization](nodes/design-without-randomization.md) | omitted variable bias를 우회하는 external variation을 설명한다. |
| 09 Non Compliance and LATE | not created | [design-without-randomization](nodes/design-without-randomization.md) | effect 대상이 complier로 좁아지는 이유를 설명한다. |
| 10 Matching | not created | [design-without-randomization](nodes/design-without-randomization.md) | 비슷한 사람끼리 비교한다는 직관과 한계를 잡는다. |
| 11 Propensity Score | not created | [design-without-randomization](nodes/design-without-randomization.md) | treatment probability를 balancing score로 쓴다. |
| 12 Doubly Robust Estimation | not created | [design-without-randomization](nodes/design-without-randomization.md) | outcome model과 propensity model을 함께 쓰는 이유를 설명한다. |
| 13 Difference-in-Differences | not created | [panel-time](nodes/panel-time.md) | before-after와 treated-control을 동시에 비교한다. |
| 14 Panel Data and Fixed Effects | not created | [panel-time](nodes/panel-time.md) | 보이지 않는 고정 차이를 제거한다. |
| 15 Synthetic Control | not created | [panel-time](nodes/panel-time.md), [inference](nodes/inference.md) | control units의 가중 평균으로 counterfactual을 만든다. |
| 16 Regression Discontinuity Design | not created | [panel-time](nodes/panel-time.md) | cutoff 주변의 국소 비교를 사용한다. |
| 17 Predictive Models 101 | not created | [prediction-policy](nodes/prediction-policy.md) | prediction을 policy input으로 제한해서 읽는다. |
| 18 Heterogeneous Treatment Effects | not created | [heterogeneity](nodes/heterogeneity.md) | 평균 효과에서 개인별 효과 함수로 이동한다. |
| 19 Evaluating Causal Models | not created | [heterogeneity](nodes/heterogeneity.md), [inference](nodes/inference.md) | causal ranking과 policy gain으로 평가한다. |
| 20 Plug-and-Play Estimators | not created | [heterogeneity](nodes/heterogeneity.md) | target transformation으로 ML 모델을 causal estimator처럼 쓴다. |
| 21 Meta Learners | not created | [heterogeneity](nodes/heterogeneity.md) | S, T, X learner를 data regime별 선택지로 정리한다. |
| 22 Debiased Orthogonal ML | not created | [orthogonal-ml](nodes/orthogonal-ml.md) | nuisance parameter 추정과 target effect 추정을 분리한다. |
| 23 Effect Heterogeneity and Nonlinearity | not created | [heterogeneity](nodes/heterogeneity.md), [orthogonal-ml](nodes/orthogonal-ml.md) | nonlinear outcome과 binary outcome에서 effect 해석이 흔들리는 지점을 잡는다. |
| 24 Difference-in-Differences Saga | not created | [modern-did-sdid](nodes/modern-did-sdid.md) | heterogeneous effects가 classic DID를 망가뜨리는 이유를 설명한다. |
| 25 Synthetic Difference-in-Differences | not created | [modern-did-sdid](nodes/modern-did-sdid.md) | DID와 synthetic control을 결합한 비교 설계를 설명한다. |
| Debiasing with Orthogonalization | not created | [orthogonal-ml](nodes/orthogonal-ml.md) | orthogonalization 직관을 linear regression에서 다시 설명한다. |
| Debiasing with Propensity Score | not created | [design-without-randomization](nodes/design-without-randomization.md) | IPTW, stored score, estimated score, positivity를 정리한다. |
| When Prediction Fails | not created | [prediction-policy](nodes/prediction-policy.md) | 좋은 prediction이 나쁜 intervention policy를 만들 수 있음을 설명한다. |
| Prediction Metrics For Causal Models | not created | [prediction-policy](nodes/prediction-policy.md), [inference](nodes/inference.md) | prediction metric이 causal model 평가를 왜 오도하는지 설명한다. |
| Conformal Inference for Synthetic Controls | not created | [inference](nodes/inference.md) | synthetic control에서 p-value와 confidence interval을 구성한다. |
| Simulated-Data | support, outside toc | [route](route.md) | 예제 데이터 생성 자료다. 본문 route에는 넣지 않는다. |

## Korean Scope

한국어 노트북은 현재 모두 삭제된 상태다.

다시 만들 때는 원본 30개 목차 파일 전체를 대상으로 하되, 바로 번역하지 말고 해당 노드의 `Student Bridge`와 `Rewrite Focus`를 먼저 적용한다.
