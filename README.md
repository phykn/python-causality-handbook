# Causal Inference for The Brave and True: 한국어 강의노트

데이터를 보면 두 숫자가 함께 움직일 때가 많습니다.

비싼 마우스를 쓰는 사람이 승률도 높고, 쿠폰을 받은 사람이 더 많이 구매하고, 정책을 받은 지역의 지표가 좋아질 수 있습니다. 하지만 같이 움직인다고 해서 한쪽이 다른 쪽을 바꾸었다고 바로 말할 수는 없습니다.

이 노트는 그 차이를 차근차근 따져 보는 한국어 강의노트입니다.

중심 질문은 항상 같습니다.

```text
무엇과 무엇을 비교했는가?
그 비교를 인과 효과로 읽으려면 무엇이 비슷해야 하는가?
그래도 남는 의심은 무엇인가?
```

공식보다 비교를 먼저 봅니다. 방법 이름은 필요가 보인 뒤에 붙입니다. 각 장은 가능한 한 작은 숫자, 표, 짧은 코드로 비교가 어떻게 만들어지는지 보여 줍니다.

원본은 [Causal Inference for The Brave and True](https://matheusfacure.github.io/python-causality-handbook/landing-page.html)입니다. 이 저장소의 `ko/` 문서는 원문을 그대로 옮긴 번역이 아니라, 한국어 독자가 따라 읽기 쉽도록 다시 쓴 강의노트입니다.

## 읽는 법

처음 읽는다면 1장부터 순서대로 읽는 것이 좋습니다. 앞 장에서 만든 비교 감각이 뒤 장의 도구로 이어집니다.

이미 인과추론을 조금 알고 있다면 관심 있는 묶음부터 읽어도 됩니다.

- 1~3장: 인과 질문과 추정값의 불확실성
- 4~9장: 비교가 왜 망가지는지
- 10~18장: 실험 없이 비교를 만드는 방법
- 19~25장: 예측 모델을 정책과 개인별 효과로 연결하는 방법
- 26~28장: 시간 자료, synthetic control, 효과 범위

## 목차

### 1부. 인과 질문 세우기

- [1장. 상관관계와 인과관계는 왜 다른가](ko/01-correlation-vs-causation.md)
- [2장. 무작위 실험이 공정한 비교를 만드는 이유](ko/02-randomized-experiments.md)
- [3장. 추정값은 왜 매번 달라지는가](ko/03-why-estimates-vary.md)

### 2부. 비교가 망가지는 이유

- [4장. 숨은 이유가 평균 차이에 섞이는 방식](ko/04-hidden-causes-confounding.md)
- [5장. 선택 편향은 왜 교란요인과 다른가](ko/05-selection-bias.md)
- [6장. 인과 그래프는 무엇을 맞출지 정리하는 도구다](ko/06-causal-graphs.md)
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

- [26장. 먼저 설치한 곳을 비교 대상으로 써도 될까](ko/26-did-with-staggered-adoption.md)
- [27장. 비교 대상을 맞추고 시간 변화도 뺀다](ko/27-synthetic-difference-in-differences.md)
- [28장. 한 숫자만 말하면 너무 단정적이다](ko/28-conformal-inference-synthetic-control.md)

## 출처

- [Causal Inference for The Brave and True](https://matheusfacure.github.io/python-causality-handbook/landing-page.html)
- [matheusfacure/python-causality-handbook](https://github.com/matheusfacure/python-causality-handbook)
