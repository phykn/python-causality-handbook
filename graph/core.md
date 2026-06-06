# Core

이 책의 중심은 "상관관계를 보고 정책 결정을 해도 되는가"라는 질문이다.

예측 문제는 `무엇이 일어날까`를 묻는다. 인과 문제는 `무언가를 바꾸면 무엇이 달라질까`를 묻는다. 한국어 강의노트는 이 차이를 계속 보이게 해야 한다.

## Audience Aim

목표 독자는 중/고등학생이다.

독자가 미적분, 선형대수, 대학 통계학, 머신러닝을 이미 안다고 가정하지 않는다. 대신 다음 순서로 설명한다.

1. 생활 속 선택 상황을 먼저 둔다.
2. 두 선택지를 비교하는 말로 바꾼다.
3. 왜 그 비교가 공정하거나 불공정한지 묻는다.
4. 필요한 용어를 그때 붙인다.
5. 수식과 코드는 이미 설명한 비교를 확인하는 도구로 놓는다.

학생이 이해해야 할 핵심은 모든 공식을 외우는 것이 아니다. `이 비교를 믿어도 되는가`를 스스로 물을 수 있게 되는 것이다.

## Central Claim

인과추론은 더 복잡한 모델을 찾는 일이 아니라, 비교가 믿을 만한 조건을 만드는 일이다.

모델은 그 조건을 표현하거나 보정하거나 검증하는 도구다. 모델 자체가 인과성을 만들지는 않는다.

## Three Questions

1. `What is the causal contrast?`
   - 어떤 처치를 비교하는가.
   - 어떤 결과가 바뀌어야 하는가.
   - 비교 대상은 관측 가능한가, 반사실인가.

2. `Why can this comparison be trusted?`
   - 무작위 배정인가.
   - 관측 변수로 조정 가능한가.
   - 도구변수, 시간 변화, 절단점, synthetic control 같은 설계가 필요한가.

3. `What does this estimate support?`
   - 평균 효과만 필요한가.
   - 개인별 효과나 정책 타게팅이 필요한가.
   - 불확실성과 모델 평가가 결정을 바꿀 만큼 중요한가.

## Rewrite Principle

각 장은 기법 이름으로 시작하지 않는다. 독자가 처한 판단 문제로 시작한다.

나쁜 시작:

- `이번 장에서는 propensity score를 배운다.`

좋은 시작:

- `처치받은 사람과 받지 않은 사람이 애초에 다르면, 우리는 어떤 비교를 믿을 수 있을까?`

학생용 좋은 시작:

- `학원을 다닌 학생의 성적이 더 높다면, 학원이 성적을 올렸다고 바로 말해도 될까? 아니면 애초에 공부를 더 좋아하는 학생들이 학원에 갔을까?`

## Graph Edges

- Start at [foundation](nodes/foundation.md).
- If the comparison is distorted by observed or unobserved causes, go to [causal-graphs](nodes/causal-graphs.md).
- If adjustment by observed variables is plausible, go to [regression-adjustment](nodes/regression-adjustment.md).
- If adjustment alone is not enough, go to [design-without-randomization](nodes/design-without-randomization.md) or [panel-time](nodes/panel-time.md).
- If the decision needs personalization, go to [prediction-policy](nodes/prediction-policy.md), [heterogeneity](nodes/heterogeneity.md), and [orthogonal-ml](nodes/orthogonal-ml.md).
- If the design is time-staggered or heterogeneous, go to [modern-did-sdid](nodes/modern-did-sdid.md).
- Use [inference](nodes/inference.md) whenever uncertainty changes the decision.
