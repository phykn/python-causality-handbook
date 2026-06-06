# Prediction Policy

## Question

예측 모델은 언제 정책 결정에 도움이 되고, 언제 위험해지는가?

## Reader State

독자는 ML을 성능 좋은 prediction tool로 알고 있다. 이 노드는 prediction을 intervention policy의 입력으로 사용할 때 생기는 차이를 보여준다.

## Core Idea

prediction model은 `누가 높은 outcome을 가질까`를 잘 맞힐 수 있다. 그러나 policy는 `누구에게 intervention을 하면 outcome이 바뀔까`를 묻는다.

따라서 prediction metric은 causal model 품질을 보장하지 않는다. 정책 이득, treatment effect ranking, cumulative gain 같은 평가가 필요하다.

## Student Bridge

학생에게는 prediction과 policy를 시험 예시로 분리한다. "누가 시험을 잘 볼까"와 "누구에게 보충수업을 주면 점수가 오를까"는 다른 질문이다.

추가 설명이 필요한 부분:

- prediction: 앞으로 나올 결과를 맞히는 일.
- policy: 누구에게 무엇을 할지 정하는 규칙.
- intervention: 결과를 바꾸려고 하는 행동.
- ranking: 먼저 도와야 할 대상을 순서대로 놓는 일.
- gain: 그 순서가 실제로 얼마나 도움이 되는지 보는 값.

## Source Chapters

- 17 Predictive Models 101
- 19 Evaluating Causal Models
- When Prediction Fails
- Prediction Metrics For Causal Models

## Edges

- Previous: [panel-time](panel-time.md)
- Next: [heterogeneity](heterogeneity.md)
- Cross-link: [inference](inference.md)

## Rewrite Focus

한국어 장은 ML 개론으로 흐르면 안 된다. ML은 policy decision을 위한 input으로 제한해서 설명한다.

설명 순서:

1. prediction problem과 treatment assignment problem을 비교한다.
2. 좋은 prediction이 나쁜 policy를 만들 수 있는 상황을 보인다.
3. one-feature policy에서 fine-grain policy로 이동한다.
4. causal model 평가가 prediction metric과 다른 이유를 설명한다.
5. 다음 질문으로 CATE를 도입한다.

## Common Failure

정확도, RMSE, AUC 같은 metric을 중심에 두면 이 노드는 원문 의도와 어긋난다. 중심 metric은 intervention decision의 품질이다.
