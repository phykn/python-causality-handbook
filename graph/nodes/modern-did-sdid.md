# Modern DID And SDID

## Question

treatment effect가 시간과 집단마다 다르면 기존 DID와 synthetic control은 어떻게 바뀌어야 하는가?

## Reader State

독자는 classic DID, fixed effects, synthetic control을 배웠다. 이제 heterogeneous effect와 staggered adoption이 기존 estimator를 왜 흔드는지 본다.

## Core Idea

classic DID는 parallel trends와 stable effect intuition에 기대지만, treatment effect heterogeneity가 있으면 TWFE 계수가 해석하기 어려워질 수 있다.

modern DID는 더 유연한 functional form과 event-study 사고를 사용해 이 문제를 드러낸다.

SDID는 DID의 time comparison과 synthetic control의 weighted comparison을 결합한다.

## Student Bridge

학생에게는 modern DID를 "어려운 DID"로 소개하지 않는다. "처치 효과가 모두에게 같은 크기라고 생각하면 어떤 실수를 하는가"로 시작한다.

추가 설명이 필요한 부분:

- TWFE: unit 차이와 time 차이를 함께 빼는 회귀 방식.
- event study: 처치 전후 여러 시점을 나눠 변화 모양을 보는 방법.
- staggered adoption: 각 집단이 서로 다른 시점에 처치를 받기 시작하는 상황.
- effect heterogeneity in time: 시간이 지나며 효과 크기가 달라지는 현상.
- SDID: 시간 비교와 synthetic control 비교를 함께 쓰는 방법.

## Source Chapters

- 24 Difference-in-Differences Saga
- 25 Synthetic Difference-in-Differences

## Edges

- Previous: [orthogonal-ml](orthogonal-ml.md)
- Back-link: [panel-time](panel-time.md)
- Cross-link: [inference](inference.md)

## Rewrite Focus

한국어 장은 "DID 심화"가 아니라 "기존 DID 직관이 언제 죽고 어떻게 다시 살아나는가"로 구성한다.

설명 순서:

1. classic DID가 약속했던 쉬운 비교를 복기한다.
2. effect heterogeneity가 TWFE를 왜 망가뜨리는지 보인다.
3. event study가 어떤 failure를 드러내는지 설명한다.
4. flexible functional form이 어떤 비교를 회복하는지 보인다.
5. SDID가 synthetic control과 DID를 왜 결합하는지 설명한다.

## Current Korean Gap

`25-Synthetic-Diff-in-Diff.ipynb`는 한국어 노트북을 다시 만들 때 이 노드를 먼저 읽고 새 장으로 만들어야 한다.

## Common Failure

이 노드를 estimator update history로 쓰면 안 된다. 핵심은 time design에서 treatment effect heterogeneity가 식별과 해석을 바꾸는 방식이다.
