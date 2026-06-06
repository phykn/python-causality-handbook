# Orthogonal ML

## Question

flexible ML을 쓰면서도 treatment effect estimate의 bias를 어떻게 줄일 수 있는가?

## Reader State

독자는 ML이 outcome이나 propensity 같은 nuisance function을 잘 추정할 수 있음을 안다. 그러나 그 ML 오차가 causal target에 들어오면 문제가 된다는 점을 배운다.

## Core Idea

orthogonalization은 nuisance model의 작은 추정 오차가 target parameter에 직접적인 first-order bias를 만들지 않도록 설계를 바꾼다.

Double ML은 nuisance estimation과 target effect estimation을 분리하고, cross-fitting으로 overfitting의 영향을 줄인다.

## Student Bridge

학생에게는 orthogonalization을 수학 단어로 시작하지 않는다. "먼저 설명할 수 있는 부분을 빼고, 남은 차이끼리 비교한다"로 시작한다.

추가 설명이 필요한 부분:

- nuisance model: 직접 알고 싶은 효과는 아니지만 보정에 필요한 예측 모델.
- residualization: 이미 설명된 부분을 빼고 남기는 일.
- orthogonalization: 남은 차이가 보정 모델의 작은 실수에 덜 흔들리게 만드는 설계.
- cross-fitting: 데이터를 나눠서 한쪽으로 배우고 다른 쪽으로 확인하는 방식.
- debiasing: 잘못된 방향으로 치우친 estimate를 줄이는 일.

## Source Chapters

- 22 Debiased Orthogonal Machine Learning
- Debiasing with Orthogonalization
- 23 Challenges with Effect Heterogeneity and Nonlinearity

## Edges

- Previous: [heterogeneity](heterogeneity.md)
- Next: [modern-did-sdid](modern-did-sdid.md)
- Cross-link: [regression-adjustment](regression-adjustment.md)
- Cross-link: [design-without-randomization](design-without-randomization.md)

## Rewrite Focus

한국어 장은 수식을 숨기지 않되, 먼저 왜 orthogonalization이 필요한지 보여줘야 한다.

설명 순서:

1. flexible ML이 nuisance prediction에는 좋지만 target effect에는 bias를 만들 수 있음을 보인다.
2. residualization 또는 partialling out 직관을 regression에서 시작한다.
3. Frisch-Waugh-Lovell을 "남은 variation끼리 비교한다"로 설명한다.
4. Double ML과 cross-fitting이 같은 직관을 확장한다는 점을 보인다.
5. non-parametric과 non-scientific use의 경계를 남긴다.

## Common Failure

orthogonal ML을 최신 ML 기법으로만 소개하면 안 된다. 이 노드는 identification을 보존하면서 flexible nuisance model을 쓰는 방법이다.
