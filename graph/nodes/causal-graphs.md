# Causal Graphs

## Question

비교가 왜 망가지는지 어떻게 볼 수 있는가?

## Reader State

독자는 treatment와 outcome 사이의 association을 봤지만, 그 association이 causal effect인지 확신하지 못한다.

## Core Idea

causal graph는 변수 사이의 방향 있는 관계를 그려서 bias path를 찾는 도구다.

confounding은 treatment와 outcome에 함께 영향을 주는 원인이 비교를 오염시키는 문제다. selection은 어떤 값을 조건으로 잡는 순간 원래 없던 관계가 생기거나 필요한 비교가 사라지는 문제다.

control은 많이 넣는 것이 아니라, 어떤 path를 닫고 어떤 path를 열지 판단해서 고른다.

## Student Bridge

학생에게는 graph를 수학 기호로 시작하지 않는다. "화살표는 한 일이 다른 일을 바꿀 수 있다는 표시"라고 시작한다.

추가 설명이 필요한 부분:

- confounder: 원인처럼 보이는 것과 결과를 둘 다 움직이는 배경 이유.
- path: 화살표를 따라 이어지는 길.
- selection: 비교할 사람을 고르는 방식 때문에 이미 생긴 차이.
- collider: 두 이유가 함께 모이는 지점을 골라서 없던 관계를 만드는 상황.
- control: 비교를 공정하게 만들기 위해 잠시 같다고 보는 변수.

## Source Chapters

- 04 Graphical Causal Models
- 07 Beyond Confounders

## Edges

- Previous: [foundation](foundation.md)
- Next: [regression-adjustment](regression-adjustment.md)
- Alternative route: [design-without-randomization](design-without-randomization.md)

## Rewrite Focus

한국어 설명은 그래프 용어보다 "어떤 비교가 오염되는가"를 먼저 보여준다.

설명 순서:

1. treatment와 outcome 사이에 보이는 association을 놓는다.
2. 제3의 원인이 두 변수에 동시에 영향을 주는 상황을 그린다.
3. confounder를 control하면 무엇이 좋아지는지 보인다.
4. collider나 mediator를 control하면 왜 오히려 망가지는지 보인다.
5. good control, bad control, harmful control을 사례별로 정리한다.

## Common Failure

DAG 문법을 먼저 가르치면 독자는 왜 그래프가 필요한지 놓친다. 그래프는 시각 자료가 아니라 bias diagnosis다.
