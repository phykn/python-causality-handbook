# Explanation Gaps

이 문서는 중/고등학생 독자에게 추가 설명이 필요한 부분을 모은다.

각 항목은 해당 장을 다시 쓸 때 먼저 보강해야 하는 설명이다. 원문에 있는 용어를 그대로 번역하기 전에, 학생이 어떤 오해를 할 수 있는지 확인한다.

## Foundation

Source:

- `01-Introduction-To-Causality.ipynb`
- `02-Randomised-Experiments.ipynb`
- `03-Stats-Review-The-Most-Dangerous-Equation.ipynb`

Needs bridge:

- `상관관계`: 두 일이 함께 보이는 것.
- `인과관계`: 하나를 바꾸면 다른 것이 달라지는 것.
- `반사실`: 실제로 보지 못한 다른 선택의 결과.
- `무작위 배정`: 비교할 두 집단을 공정하게 만드는 장치.
- `표준오차`: 같은 실험을 다시 하면 estimate가 얼마나 흔들릴지 나타내는 크기.

Student example:

- 같은 반 학생 중 학원을 다닌 학생의 평균 점수가 높다. 이 차이가 학원 때문인지, 원래 공부 시간이 긴 학생들이 학원에 갔기 때문인지 묻는다.

## Causal Graphs And Controls

Source:

- `04-Graphical-Causal-Models.ipynb`
- `07-Beyond-Confounders.ipynb`

Needs bridge:

- `confounder`: 원인과 결과 양쪽에 영향을 주는 숨은 이유.
- `selection`: 비교 대상이 고르는 과정에서 이미 달라지는 문제.
- `collider`: 두 원인이 함께 모이는 지점을 조건으로 잡아 새 관계를 만드는 문제.
- `control`: 무조건 넣는 변수가 아니라, 비교를 공정하게 만들기 위해 고르는 변수.

Student example:

- 운동을 많이 하는 학생이 성적도 높다고 해서 운동이 성적을 올렸다고 말할 수 없다. 시간 관리 능력이 운동과 성적 모두에 영향을 줄 수 있다.

## Regression And Adjustment

Source:

- `05-The-Unreasonable-Effectiveness-of-Linear-Regression.ipynb`
- `06-Grouped-and-Dummy-Regression.ipynb`

Needs bridge:

- `회귀`: 비슷한 조건을 가진 사람끼리 평균을 비교하는 계산 도구.
- `계수`: 다른 조건을 고정했을 때 한 변수가 바뀌면 결과가 얼마나 달라지는지 요약한 숫자.
- `dummy variable`: 집단 이름을 0과 1로 표시하는 방법.
- `residual`: 설명하고 남은 차이.

Student example:

- 학원 효과를 보려면 공부 시간, 이전 성적, 학년이 비슷한 학생끼리 비교해야 한다.

## Non-Random Designs

Source:

- `08-Instrumental-Variables.ipynb`
- `09-Non-Compliance-and-LATE.ipynb`
- `10-Matching.ipynb`
- `11-Propensity-Score.ipynb`
- `12-Doubly-Robust-Estimation.ipynb`
- `Debiasing-with-Propensity-Score.ipynb`

Needs bridge:

- `instrument`: 직접 원인은 아니지만 treatment를 움직이는 외부 이유.
- `first stage`: instrument가 treatment를 실제로 움직이는지 확인하는 단계.
- `LATE`: treatment를 따르게 된 사람들에게만 적용되는 효과.
- `matching`: 비슷한 사람끼리 짝지어 비교하는 방법.
- `propensity score`: treatment를 받을 가능성.
- `positivity`: 비교할 양쪽 사람이 모두 실제로 존재해야 한다는 조건.
- `doubly robust`: 두 가지 보정 중 하나가 맞으면 버틸 수 있는 방식.

Student example:

- 학교가 무작위로 보충수업 초대장을 보냈지만, 초대받은 학생 중 일부만 실제로 참여했다. 초대장은 보충수업 참여를 움직이는 도구가 될 수 있다.

## Time And Natural Boundaries

Source:

- `13-Difference-in-Differences.ipynb`
- `14-Panel-Data-and-Fixed-Effects.ipynb`
- `15-Synthetic-Control.ipynb`
- `16-Regression-Discontinuity-Design.ipynb`

Needs bridge:

- `parallel trends`: 처치가 없었다면 두 집단이 비슷한 방향으로 변했을 것이라는 생각.
- `fixed effects`: 각 사람이나 지역이 원래 가진 변하지 않는 차이를 제거하는 방법.
- `synthetic control`: 여러 비교 대상을 섞어 가상의 비교 대상을 만드는 방법.
- `cutoff`: 어떤 규칙이 바뀌는 경계점.
- `RDD`: cutoff 바로 주변의 사람들을 비교하는 방법.

Student example:

- 장학금 기준이 80점이면, 79점과 81점 학생은 매우 비슷하지만 장학금 여부가 달라진다. 이 경계 주변을 비교한다.

## Prediction, Policy, And Heterogeneity

Source:

- `17-Predictive-Models-101.ipynb`
- `18-Heterogeneous-Treatment-Effects-and-Personalization.ipynb`
- `19-Evaluating-Causal-Models.ipynb`
- `20-Plug-and-Play-Estimators.ipynb`
- `21-Meta-Learners.ipynb`
- `When-Prediction-Fails.ipynb`
- `Prediction-Metrics-For-Causal-Models.ipynb`

Needs bridge:

- `prediction`: 앞으로 어떤 결과가 나올지 맞히는 일.
- `policy`: 누구에게 어떤 행동을 할지 정하는 규칙.
- `ATE`: 전체 평균 효과.
- `CATE`: 특성이 비슷한 사람들의 효과.
- `uplift`: intervention을 했기 때문에 더 좋아진 정도.
- `model evaluation`: 예측 정확도가 아니라 좋은 결정을 만드는지 평가하는 일.

Student example:

- 시험을 이미 잘 볼 학생을 맞히는 모델과, 추가 수업을 들으면 점수가 오를 학생을 찾는 모델은 다르다.

## Orthogonal ML And Modern DID

Source:

- `22-Debiased-Orthogonal-Machine-Learning.ipynb`
- `23-Challenges-with-Effect-Heterogeneity-and-Nonlinearity.ipynb`
- `24-The-Diff-in-Diff-Saga.ipynb`
- `25-Synthetic-Diff-in-Diff.ipynb`
- `Debiasing-with-Orthogonalization.ipynb`
- `Conformal-Inference-for-Synthetic-Control.ipynb`

Needs bridge:

- `nuisance model`: 직접 알고 싶은 효과는 아니지만 보정에 필요한 예측 모델.
- `orthogonalization`: 먼저 설명할 수 있는 부분을 빼고, 남은 차이끼리 비교하는 생각.
- `cross-fitting`: 같은 데이터로 배우고 평가하는 문제를 줄이기 위해 데이터를 나눠 쓰는 방법.
- `effect heterogeneity`: 효과가 사람이나 시간마다 달라지는 현상.
- `staggered adoption`: 처치가 모든 집단에 같은 시점에 시작되지 않는 상황.
- `conformal inference`: 데이터가 보여준 오차 패턴을 이용해 가능한 결과 범위를 만드는 방법.

Student example:

- 선생님이 각 학생의 원래 실력과 공부 시간을 먼저 예측해 본 뒤, 그래도 남는 차이가 보충수업 때문인지 비교한다.
