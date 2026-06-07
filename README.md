# Causal Inference for The Brave and True: 한국어 강의노트

인과추론은 데이터에서 "무엇이 무엇을 일으켰는가"를 묻는 방법입니다. 예측이 앞으로 일어날 값을 맞히는 일에 가깝다면, 인과추론은 어떤 선택이나 개입이 결과를 어떻게 바꾸는지 따집니다. 그래서 단순히 두 값이 같이 움직인다는 사실만으로는 부족합니다. 비교가 공정했는지, 보이지 않는 이유가 섞였는지, 우리가 실제로 알고 싶은 반사실적 질문이 무엇인지 계속 확인해야 합니다.

이 저장소는 `Causal Inference for The Brave and True`를 참고해 다시 쓰는 한국어 강의노트입니다. 원문을 문장별로 옮기는 번역본이 아니라, 인과추론을 처음 접하는 한국어 독자가 한 장씩 따라 읽을 수 있도록 예시와 설명 순서를 새로 잡은 독립적인 글을 목표로 합니다.

각 장은 익숙한 상황에서 시작해, 왜 단순한 평균 차이나 상관관계가 위험한지 먼저 보여줍니다. 그 다음에 무작위 실험, 교란요인, 선택 편향, 회귀, 매칭, 성향점수 같은 도구가 어떤 문제를 풀기 위해 필요한지 붙입니다.

목표는 어려운 내용을 빼는 것이 아닙니다. 먼저 독자가 붙잡을 수 있는 질문과 비교 대상을 세우고, 그 뒤에 필요한 용어와 수식, 파이썬 코드를 올리는 것입니다. 이 노트는 인과추론을 "기법 목록"이 아니라, 좋은 비교를 만들기 위한 사고방식으로 읽도록 돕습니다.

## 목차

1. [상관관계와 인과관계는 왜 다른가](ko/01-correlation-vs-causation.md)
2. [무작위 실험이 강한 이유](ko/02-randomized-experiments.md)
3. [추정값은 왜 흔들리는가](ko/03-why-estimates-vary.md)
4. [숨은 이유가 평균 차이에 섞이는 방식](ko/04-hidden-causes-confounding.md)
5. [선택 편향은 왜 교란요인과 다른가](ko/05-selection-bias.md)
6. [그래프로 원인과 비교를 그려보기](ko/06-causal-graphs.md)
7. [회귀를 조건부 비교로 읽기](ko/07-regression-adjustment.md)
8. [더미 변수와 집단 비교](ko/08-dummy-variables.md)
9. [좋은 통제와 나쁜 통제](ko/09-good-bad-controls.md)
10. [관측 자료에서 비교 대상을 찾는다는 것](ko/10-matching.md)
11. [처치받을 가능성으로 균형 맞추기](ko/11-propensity-score.md)
12. [두 모델을 함께 쓰면 무엇이 나아질까](ko/12-doubly-robust-estimation.md)
13. [전후 변화만 보면 왜 부족할까](ko/13-difference-in-differences.md)
14. [같은 PC방을 여러 번 보면 무엇을 뺄 수 있을까](ko/14-panel-data-fixed-effects.md)
15. [비교할 PC방이 하나도 딱 맞지 않다면](ko/15-synthetic-control.md)

## 출처

- [Causal Inference for The Brave and True](https://matheusfacure.github.io/python-causality-handbook/landing-page.html)
- [matheusfacure/python-causality-handbook](https://github.com/matheusfacure/python-causality-handbook)
