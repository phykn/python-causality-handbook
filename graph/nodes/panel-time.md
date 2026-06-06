# Panel Time

## Question

시간, 반복 관측, cutoff를 이용하면 어떤 비교를 만들 수 있는가?

## Reader State

독자는 cross-section 조정과 matching 계열의 한계를 안다. 이제 같은 단위의 시간 변화나 제도적 절단점을 이용해 비교를 만든다.

## Core Idea

시간 구조는 보이지 않는 차이를 제거하거나 counterfactual trend를 구성하는 데 쓸 수 있다.

- DID는 treated-control 차이와 before-after 차이를 함께 사용한다.
- fixed effects는 시간에 따라 변하지 않는 unit-level confounder를 제거한다.
- synthetic control은 control units의 가중 평균으로 treated unit의 counterfactual path를 만든다.
- RDD는 cutoff 주변의 국소 무작위성에 기대어 비교한다.

## Student Bridge

학생에게는 time design을 "전후 비교"로만 설명하면 안 된다. 먼저 전후 비교가 왜 속을 수 있는지 보여준다.

추가 설명이 필요한 부분:

- parallel trends: 처치가 없었다면 두 집단이 비슷한 방향으로 움직였을 것이라는 생각.
- fixed effects: 사람이나 지역이 원래 가진 변하지 않는 차이를 빼는 방법.
- synthetic control: 여러 비교 대상을 섞어 만든 가상의 비교 대상.
- cutoff: 규칙이 바뀌는 경계점.
- local comparison: cutoff 바로 주변처럼 매우 비슷한 대상끼리 하는 비교.

## Source Chapters

- 13 Difference-in-Differences
- 14 Panel Data and Fixed Effects
- 15 Synthetic Control
- 16 Regression Discontinuity Design

## Edges

- Previous: [design-without-randomization](design-without-randomization.md)
- Next: [prediction-policy](prediction-policy.md)
- Later revision: [modern-did-sdid](modern-did-sdid.md)
- Cross-link: [inference](inference.md)

## Rewrite Focus

한국어 설명은 "시간이 있으면 자동으로 인과가 된다"는 오해를 막아야 한다.

설명 순서:

1. 시간 전후 비교만으로 왜 부족한지 보인다.
2. treated-control 비교만으로 왜 부족한지 보인다.
3. 두 비교를 결합하면 어떤 bias가 제거되는지 보인다.
4. parallel trends, no extrapolation, cutoff continuity 같은 method-specific assumption을 붙인다.
5. assumption이 깨지는 사례를 다음 장의 질문으로 남긴다.

## Common Failure

시계열 그림이 설득력 있어 보여도 identification assumption을 대신하지 않는다. 그래프와 문장은 항상 assumption을 같이 보여줘야 한다.
