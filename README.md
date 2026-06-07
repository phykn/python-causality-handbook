# Causal Inference for The Brave and True: 한국어 강의노트

인과추론은 어떤 선택이나 행동이 결과를 실제로 바꾸었는지 따져 보는 방법입니다.

데이터를 보면 두 일이 함께 나타날 때가 많습니다. 하지만 함께 나타난다고 해서 한쪽이 다른 쪽의 원인이라고 바로 말할 수는 없습니다.

그래서 인과추론은 비교에서 시작합니다. 누구와 누구를 비교해야 하는지, 그 비교를 믿으려면 무엇이 비슷해야 하는지, 그래도 남는 의심은 무엇인지 차례대로 살펴봅니다.

이 저장소는 `Causal Inference for The Brave and True`를 참고해 작성하는 한국어 강의노트입니다.

## 목차

### 1부. 인과 질문 세우기

- [1장. 상관관계와 인과관계는 왜 다른가](ko/01-correlation-vs-causation.md)
- [2장. 무작위 실험이 강한 이유](ko/02-randomized-experiments.md)
- [3장. 추정값은 왜 흔들리는가](ko/03-why-estimates-vary.md)

### 2부. 비교가 망가지는 이유

- [4장. 숨은 이유가 평균 차이에 섞이는 방식](ko/04-hidden-causes-confounding.md)
- [5장. 선택 편향은 왜 교란요인과 다른가](ko/05-selection-bias.md)
- [6장. 그래프로 원인과 비교를 그려보기](ko/06-causal-graphs.md)
- [7장. 회귀를 조건부 비교로 읽기](ko/07-regression-adjustment.md)
- [8장. 더미 변수와 집단 비교](ko/08-dummy-variables.md)
- [9장. 좋은 통제와 나쁜 통제](ko/09-good-bad-controls.md)

### 3부. 실험 없이 비교 만들기

- [10장. 보이지 않는 차이가 남아 있을 때](ko/10-instrumental-variables.md)
- [11장. 쿠폰을 받았다고 모두 사는 것은 아니다](ko/11-non-compliance-and-late.md)
- [12장. 관측 자료에서 비교 대상을 찾는다는 것](ko/12-matching.md)
- [13장. 처치받을 가능성으로 균형 맞추기](ko/13-propensity-score.md)
- [14장. 두 모델을 함께 쓰면 무엇이 나아질까](ko/14-doubly-robust-estimation.md)
- [15장. 전후 변화만 보면 왜 부족할까](ko/15-difference-in-differences.md)
- [16장. 같은 PC방을 여러 번 보면 무엇을 뺄 수 있을까](ko/16-panel-data-fixed-effects.md)
- [17장. 비교할 PC방이 하나도 딱 맞지 않다면](ko/17-synthetic-control.md)
- [18장. 경계선 근처에서 비교하기](ko/18-regression-discontinuity.md)

### 4부. 예측을 정책으로 바꾸기

- [19장. 예측 모델은 언제 정책에 도움이 되는가](ko/19-prediction-policy.md)
- [20장. 평균 효과에서 개인별 효과로](ko/20-heterogeneous-treatment-effects.md)
- [21장. 누구에게 처치할지 정하는 문제](ko/21-causal-model-evaluation.md)
- [22장. 기존 머신러닝 모델로 효과 추정하기](ko/22-plug-and-play-estimators.md)
- [23장. 모델을 나눠서 효과 추정하기](ko/23-meta-learners.md)
- [24장. 먼저 설명되는 부분을 빼고 비교하기](ko/24-orthogonal-ml.md)
- [25장. 같은 도움도 위치에 따라 다르게 보인다](ko/25-effect-heterogeneity-nonlinearity.md)

### 5부. 시간 비교를 다시 점검하기

- [26장. 먼저 설치한 곳을 비교군으로 써도 될까](ko/26-did-with-staggered-adoption.md)
- [27장. 비교 대상을 맞추고 시간 변화도 뺀다](ko/27-synthetic-difference-in-differences.md)

## 출처

- [Causal Inference for The Brave and True](https://matheusfacure.github.io/python-causality-handbook/landing-page.html)
- [matheusfacure/python-causality-handbook](https://github.com/matheusfacure/python-causality-handbook)
