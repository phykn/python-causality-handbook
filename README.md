# Causal Inference for The Brave and True: 한국어 강의노트

이 저장소는 [Causal Inference for The Brave and True](https://github.com/matheusfacure/python-causality-handbook)를 참고자료로 두고, 한국어 독자를 위한 강의노트를 새로 작성하는 작업 공간이다.

목표는 번역본을 만드는 것이 아니다. 각 장은 독자가 이 페이지 안에서 질문, 예시, 실패한 비교, 공정한 비교, 방법 이름, 수식과 코드를 차례로 확인할 수 있는 독립된 한국어 글로 쓴다.

## 현재 구조

- `causal-inference-for-the-brave-and-true/`: 참고용 영어 자료.
- `ko/`: 한국어 강의노트 원고.

## 한국어 원고

- [상관관계와 인과관계는 왜 다른가](ko/01-correlation-vs-causation.md)
- [무작위 실험이 강한 이유](ko/02-randomized-experiments.md)
- [추정값은 왜 흔들리는가](ko/03-why-estimates-vary.md)

## 한국어 작성 목차

이 목차는 한국어 강의노트를 독립적으로 쓰기 위한 작성 계획이다. 독자가 인과추론을 배울 때 필요한 판단 순서에 맞춰 묶었다.

### 1부. 인과 질문 세우기

1. 상관관계와 인과관계는 왜 다른가
2. 무작위 실험이 강한 이유
3. 추정값은 왜 흔들리는가

### 2부. 비교가 망가지는 이유

6. 숨은 원인이 비교를 속이는 방식
7. 선택 편향은 왜 confounding과 다른가
8. 그래프로 원인과 비교를 그려보기
9. 회귀를 조건부 비교로 읽기
10. 더미 변수와 집단 비교
11. 좋은 통제와 나쁜 통제

### 3부. 실험 없이 비교 만들기

12. 관측 자료에서 비교 대상을 찾는다는 것
13. 도구변수: 처치를 움직이는 외부 변화
14. 순응하지 않는 사람과 국소 효과
15. 비슷한 사람끼리 비교하기
16. 처치받을 가능성으로 균형 맞추기
17. 두 모델로 버티는 추정
18. 시간 변화로 비교하기
19. 보이지 않는 고정 차이 제거하기
20. 가상의 비교 대상 만들기
21. 경계선 근처에서 비교하기

### 4부. 예측을 정책으로 바꾸기

22. 예측 모델은 언제 정책에 도움이 되는가
23. 평균 효과에서 개인별 효과로
24. 누구에게 처치할지 정하는 문제
25. 인과 모델은 어떻게 평가하는가
26. 기존 머신러닝 모델로 효과 추정하기
27. S/T/X learner로 개인별 효과 추정하기
28. 예측이 실패하는 정책 상황

### 5부. 유연한 모델을 안전하게 쓰기

29. 머신러닝이 인과추론에서 만드는 편향
30. nuisance 모델과 target 효과 구분하기
31. orthogonalization 직관
32. cross-fitting은 왜 필요한가
33. 비선형성과 이질적 효과의 함정
34. DID가 깨지는 이유와 현대 DID
35. Synthetic DID
36. Synthetic control의 불확실성

## 작성 기준

각 장은 다음 흐름으로 쓴다.

1. 독자가 혹할 만한 판단 상황
2. 지금 결론을 내리면 왜 위험한지
3. 쉬운 비교가 숨기는 것
4. 작은 숫자나 표로 착각이 깨지는 장면
5. 필요한 이름과 핵심 용어
6. 같은 말을 기호로 쓰는 장면
7. 직접 계산하거나 섞어 보는 코드
8. 한계와 오해하기 쉬운 지점
9. 다음 장으로 넘어가는 질문
10. 문서 전체의 한 줄 요약

소제목은 `용어`, `수식`, `코드` 같은 분류명이 아니라 장면 전환 문구처럼 쓴다.

## 참고

- [참고 책 웹사이트](https://matheusfacure.github.io/python-causality-handbook/landing-page.html)
- [참고 GitHub 저장소](https://github.com/matheusfacure/python-causality-handbook)
- [공식 한국어 번역](https://github.com/TeamCausality/Causal-Inference-with-Python)
