# Design Without Randomization

## Question

무작위 실험이 없고 단순 조정도 부족하면, 어떤 설계가 비교를 대신 만들어주는가?

## Reader State

독자는 observed controls와 regression adjustment를 배웠지만, unobserved confounding, non-compliance, imbalance가 남는다는 것을 안다.

## Core Idea

이 노드는 non-experimental data에서 비교 가능성을 회복하는 여러 설계를 묶는다.

- IV는 treatment 자체가 아니라 treatment를 움직이는 외생적 변화를 사용한다.
- LATE는 estimate가 전체 인구가 아니라 complier에게 적용된다는 점을 분명히 한다.
- matching은 비슷한 단위를 직접 짝짓는다.
- propensity score는 treatment probability로 covariate balance를 만든다.
- doubly robust는 outcome model과 treatment model 중 하나가 맞으면 estimate가 버틸 수 있게 한다.

## Student Bridge

학생에게는 각 방법을 estimator 이름으로 구분하지 않는다. "공정한 비교를 만들 재료가 무엇인가"로 구분한다.

추가 설명이 필요한 부분:

- IV: treatment를 직접 정하지는 않지만 treatment를 움직이는 외부 이유.
- first stage: 그 외부 이유가 실제로 treatment를 움직였는지 확인하는 단계.
- LATE: 전체가 아니라 그 외부 이유 때문에 행동이 바뀐 사람들의 효과.
- matching: 비슷한 사람끼리 짝을 맞추는 방법.
- propensity score: treatment를 받을 가능성.
- positivity: 비교할 양쪽 사람이 실제 데이터에 모두 있어야 한다는 조건.
- doubly robust: 두 설명 방법 중 하나만 맞아도 크게 무너지지 않게 만드는 방법.

## Source Chapters

- 08 Instrumental Variables
- 09 Non Compliance and LATE
- 10 Matching
- 11 Propensity Score
- 12 Doubly Robust Estimation
- Debiasing with Propensity Score

## Edges

- Previous: [regression-adjustment](regression-adjustment.md)
- Next: [panel-time](panel-time.md)
- Cross-link: [orthogonal-ml](orthogonal-ml.md)

## Rewrite Focus

기법별 장을 따로 번역하더라도, 한국어 독자는 모두 같은 상위 질문 아래에서 읽어야 한다.

설명 순서:

1. `왜 지금 비교가 믿기 어려운가`를 먼저 쓴다.
2. 해당 방법이 비교 가능성을 만드는 source를 밝힌다.
3. estimate가 누구에게 적용되는지 좁힌다.
4. method-specific failure를 분명히 한다.

## Method Boundaries

| Method | Makes comparison by | Main danger |
| --- | --- | --- |
| IV | external variation | weak or invalid instrument |
| LATE | compliance type | effect target is local |
| Matching | similar observed covariates | dimensionality and hidden confounding |
| Propensity score | treatment probability balance | positivity and model misspecification |
| Doubly robust | two nuisance models | both models can still be wrong |

## Common Failure

이 노드를 "여러 estimator 모음"으로 쓰면 안 된다. 핵심은 estimator 이름이 아니라 randomization 없이 비교를 복구하는 방식의 차이다.
