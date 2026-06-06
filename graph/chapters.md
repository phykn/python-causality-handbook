# Chapters

이 문서는 각 원본 파일을 한국어 강의노트로 다시 쓸 때의 장별 질문과 다음 연결을 정리한다.

## Part I

| Source file | Chapter question | Flow | Node | Next |
| --- | --- | --- | --- | --- |
| `01-Introduction-To-Causality.ipynb` | 상관관계와 인과효과는 왜 다른 질문인가? | why bother -> prediction과 causal question 구분 -> association이 causation이 되는 조건 -> bias | [foundation](nodes/foundation.md) | 무작위 실험 |
| `02-Randomised-Experiments.ipynb` | 어떤 배정 방식이 믿을 만한 비교를 만드는가? | gold standard -> school example -> ideal experiment -> assignment mechanism | [foundation](nodes/foundation.md) | estimate uncertainty |
| `03-Stats-Review-The-Most-Dangerous-Equation.ipynb` | estimate의 흔들림을 어떻게 판단하는가? | standard error -> confidence interval -> hypothesis test -> p-value | [foundation](nodes/foundation.md), [inference](nodes/inference.md) | bias diagnosis |
| `04-Graphical-Causal-Models.ipynb` | 비교가 오염되는 경로를 어떻게 볼 것인가? | causal thinking -> graphical models -> confounding -> selection | [causal-graphs](nodes/causal-graphs.md) | regression adjustment |
| `05-The-Unreasonable-Effectiveness-of-Linear-Regression.ipynb` | 회귀는 어떻게 조건부 비교를 구현하는가? | all you need is regression -> regression theory -> non-random data -> omitted variable bias | [regression-adjustment](nodes/regression-adjustment.md) | grouped and dummy regression |
| `06-Grouped-and-Dummy-Regression.ipynb` | group과 dummy는 회귀 비교를 어떻게 보이게 하는가? | grouped data -> dummy regression | [regression-adjustment](nodes/regression-adjustment.md) | control selection |
| `07-Beyond-Confounders.ipynb` | 어떤 control은 좋고 어떤 control은 위험한가? | good controls -> harmful controls -> bad controls -> selection bias | [causal-graphs](nodes/causal-graphs.md) | IV |
| `08-Instrumental-Variables.ipynb` | 숨은 bias가 있을 때 외생적 variation을 어떻게 쓰는가? | omitted variable bias -> quarter of birth -> first stage -> reduced form -> IV by hand -> weak instruments | [design-without-randomization](nodes/design-without-randomization.md) | LATE |
| `09-Non-Compliance-and-LATE.ipynb` | treatment를 따르지 않는 사람이 있을 때 누구의 효과를 추정하는가? | heterogeneous world -> LATE -> engagement effect | [design-without-randomization](nodes/design-without-randomization.md) | matching |
| `10-Matching.ipynb` | 비슷한 사람끼리 비교하면 어떤 문제가 남는가? | regression intuition -> subclassification -> matching estimator -> matching bias -> dimensionality | [design-without-randomization](nodes/design-without-randomization.md) | propensity score |
| `11-Propensity-Score.ipynb` | treatment probability로 balance를 만들 수 있는가? | growth mindset -> propensity score -> weighting -> estimation -> standard error -> common issues -> matching | [design-without-randomization](nodes/design-without-randomization.md) | doubly robust |
| `12-Doubly-Robust-Estimation.ipynb` | outcome model과 treatment model을 같이 쓰면 무엇이 robust해지는가? | one basket problem -> doubly robust estimation | [design-without-randomization](nodes/design-without-randomization.md) | DID |
| `13-Difference-in-Differences.ipynb` | 전후 비교와 집단 비교를 결합하면 무엇을 제거할 수 있는가? | billboard example -> DID estimator -> non-parallel trends | [panel-time](nodes/panel-time.md) | fixed effects |
| `14-Panel-Data-and-Fixed-Effects.ipynb` | 반복 관측으로 보이지 않는 고정 차이를 제거할 수 있는가? | parallel trends -> unseen controls -> fixed effects -> visualization -> time effects -> limits | [panel-time](nodes/panel-time.md) | synthetic control |
| `15-Synthetic-Control.ipynb` | control unit들의 조합으로 counterfactual path를 만들 수 있는가? | time structure -> synthetic control as regression -> no extrapolation -> inference | [panel-time](nodes/panel-time.md), [inference](nodes/inference.md) | RDD |
| `16-Regression-Discontinuity-Design.ipynb` | cutoff 주변에서는 어떤 국소 비교가 가능한가? | alcohol example -> RDD estimation -> kernel weighting -> fuzzy RDD -> McCrary test | [panel-time](nodes/panel-time.md) | prediction and policy |

## Part II

| Source file | Chapter question | Flow | Node | Next |
| --- | --- | --- | --- | --- |
| `17-Predictive-Models-101.ipynb` | 예측 모델을 정책 입력으로 쓰려면 무엇이 달라지는가? | industry ML -> ML crash course -> cross validation -> predictions and policies -> one feature policy -> fine grain policy | [prediction-policy](nodes/prediction-policy.md) | HTE |
| `18-Heterogeneous-Treatment-Effects-and-Personalization.ipynb` | 평균 효과를 넘어 개인별 효과를 어떻게 생각할 것인가? | predictions to causal inference -> ATE to CATE -> sensitivity prediction | [heterogeneity](nodes/heterogeneity.md) | causal model evaluation |
| `19-Evaluating-Causal-Models.ipynb` | causal model은 prediction metric 대신 무엇으로 평가하는가? | sensitivity bands -> cumulative sensitivity -> cumulative gain -> variance | [heterogeneity](nodes/heterogeneity.md), [inference](nodes/inference.md) | plug-and-play |
| `20-Plug-and-Play-Estimators.ipynb` | ML 모델을 causal estimator처럼 쓰려면 target을 어떻게 바꾸는가? | setup -> target transformation -> continuous treatment -> nonlinear effects | [heterogeneity](nodes/heterogeneity.md) | meta learners |
| `21-Meta-Learners.ipynb` | S, T, X learner는 어떤 데이터 상황에서 다른가? | S learner -> T learner -> X learner | [heterogeneity](nodes/heterogeneity.md) | orthogonal ML |
| `22-Debiased-Orthogonal-Machine-Learning.ipynb` | nuisance ML을 쓰면서 target effect bias를 어떻게 줄이는가? | nuisance parameters -> FWL -> double ML -> non-parametric DML -> non-scientific DML | [orthogonal-ml](nodes/orthogonal-ml.md) | heterogeneity challenges |
| `23-Challenges-with-Effect-Heterogeneity-and-Nonlinearity.ipynb` | binary outcome과 nonlinear treatment에서 effect 해석은 어떻게 흔들리는가? | binary outcomes -> simulation -> continuous treatment and nonlinearity | [heterogeneity](nodes/heterogeneity.md), [orthogonal-ml](nodes/orthogonal-ml.md) | modern DID |
| `24-The-Diff-in-Diff-Saga.ipynb` | heterogeneous effects는 classic DID를 왜 무너뜨리는가? | birth -> death over heterogeneity -> event study -> flexible form | [modern-did-sdid](nodes/modern-did-sdid.md) | SDID |
| `25-Synthetic-Diff-in-Diff.ipynb` | DID와 synthetic control을 결합하면 어떤 비교가 생기는가? | DID revisited -> synthetic control revisited -> SDID -> staggered adoption -> placebo variance | [modern-did-sdid](nodes/modern-did-sdid.md) | inference |

## Appendix And Support

| Source file | Chapter question | Flow | Node | Next |
| --- | --- | --- | --- | --- |
| `Debiasing-with-Orthogonalization.ipynb` | orthogonalization 직관을 회귀에서 어떻게 다시 볼 것인가? | linear regression reborn -> intuition -> ML orthogonalization | [orthogonal-ml](nodes/orthogonal-ml.md) | chapter 22 support |
| `Debiasing-with-Propensity-Score.ipynb` | propensity score로 debiasing할 때 어떤 한계가 생기는가? | IPTW -> stored score -> estimated score -> weakness -> positivity | [design-without-randomization](nodes/design-without-randomization.md) | chapter 11 support |
| `When-Prediction-Fails.ipynb` | 좋은 prediction은 왜 나쁜 policy를 만들 수 있는가? | hammer problem -> coupon policy -> simple policy -> model policy -> failure -> graphical explanation | [prediction-policy](nodes/prediction-policy.md) | chapter 17 support |
| `Prediction-Metrics-For-Causal-Models.ipynb` | prediction metric은 causal model 평가에서 왜 위험한가? | simulated data -> predictive metric for causal inference | [prediction-policy](nodes/prediction-policy.md), [inference](nodes/inference.md) | chapter 19 support |
| `Conformal-Inference-for-Synthetic-Control.ipynb` | synthetic control에서 confidence interval을 어떻게 구성하는가? | SC refresher -> hypothesis test -> test statistic -> p-value -> confidence intervals | [inference](nodes/inference.md) | chapter 15 support |
| `Simulated-Data.ipynb` | 예제 데이터는 어떤 장의 상황을 만들기 위한 것인가? | collections email -> hospital treatment -> app engagement -> drug impact -> billboard -> lifecycle -> price and sales -> marketing email | [route](route.md) | support only |
