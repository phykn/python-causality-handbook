# Inference

## Question

estimate가 하나의 숫자로 나왔을 때, 그 숫자를 얼마나 믿고 어떤 결정을 할 수 있는가?

## Reader State

독자는 여러 estimator를 배웠지만, estimate의 uncertainty가 decision을 바꿀 수 있다는 점을 계속 확인해야 한다.

## Core Idea

inference는 모든 노드에 걸친 cross-cutting concern이다.

표준오차, confidence interval, hypothesis test, p-value는 단순 통계 절차가 아니라 estimate가 decision을 지탱할 만큼 안정적인지 묻는 도구다.

causal model evaluation과 conformal inference는 flexible model과 synthetic control에서도 같은 질문을 이어간다.

## Student Bridge

학생에게는 inference를 "공식으로 정답을 판정하는 일"로 설명하지 않는다. "이번 결과가 우연히 나온 숫자인지, 결정을 해도 될 만큼 안정적인지 묻는 일"로 설명한다.

추가 설명이 필요한 부분:

- standard error: 같은 방식으로 다시 비교하면 estimate가 흔들리는 정도.
- confidence interval: 그 흔들림을 고려했을 때 plausible한 값의 범위.
- p-value: 차이가 없다고 가정할 때 지금 같은 결과가 얼마나 낯선지 보는 값.
- placebo: 효과가 없어야 할 곳에서도 같은 결과가 나오는지 확인하는 비교.
- conformal inference: 데이터의 오차 패턴을 이용해 가능한 결과 범위를 만드는 방법.

## Source Chapters

- 03 Stats Review
- 15 Synthetic Control
- 19 Evaluating Causal Models
- Prediction Metrics For Causal Models
- Conformal Inference for Synthetic Controls

## Edges

- Back-link: [foundation](foundation.md)
- Back-link: [panel-time](panel-time.md)
- Back-link: [prediction-policy](prediction-policy.md)
- Back-link: [modern-did-sdid](modern-did-sdid.md)

## Rewrite Focus

한국어 설명은 inference를 별도 통계 복습으로 격리하지 않는다.

설명 순서:

1. estimate가 왜 sampling variation을 가지는지 보여준다.
2. confidence interval과 p-value를 decision uncertainty로 설명한다.
3. causal model evaluation에서는 prediction metric이 아니라 treatment effect ranking의 uncertainty를 본다.
4. synthetic control에서는 placebo와 conformal logic으로 counterfactual path의 uncertainty를 설명한다.

## Current Korean Gap

`Conformal-Inference-for-Synthetic-Control.ipynb`는 한국어 노트북을 다시 만들 때 synthetic control 장과 함께 이어 읽는 appendix로 설계해야 한다.

## Common Failure

통계 용어를 공식처럼 번역하면 이 노드의 기능이 사라진다. 각 통계량은 "이 estimate로 결정을 해도 되는가"에 답해야 한다.
