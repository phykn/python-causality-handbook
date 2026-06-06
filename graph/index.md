# Content Graph

이 폴더는 `Causal Inference for the Brave and True`를 한국어 강의노트로 다시 쓰기 위한 내용 그래프다.

목표 독자는 중/고등학생이다. 원문을 1:1로 옮기는 것이 아니라, 원문 전체가 어떤 질문을 차례로 해결하는지 보존하면서 학생이 따라갈 수 있는 설명 순서로 다시 구성한다.

## Read First

1. [core](core.md): 책 전체가 붙잡는 중심 질문.
2. [audience](audience.md): 중/고등학생 독자 기준과 설명 방식.
3. [route](route.md): 독자가 어떤 판단을 순서대로 배워야 하는지.
4. [chapters](chapters.md): 각 원본 장의 질문, 흐름, 다음 연결.
5. [coverage](coverage.md): 원본 장, 앞으로 만들 한국어 장, 그래프 노드의 대응.
6. [section-coverage](section-coverage.md): 원본 노트북 heading 전체의 색인.
7. [explanation-gaps](explanation-gaps.md): 학생에게 추가 설명이 필요한 개념.
8. [rewrite-process](rewrite-process.md): 각 장을 한국어 강의노트로 바꾸는 작업 절차.

## Main Nodes

- [foundation](nodes/foundation.md): 인과 질문, 무작위 실험, 추정 불확실성.
- [causal-graphs](nodes/causal-graphs.md): 그래프, confounding, selection, control 선택.
- [regression-adjustment](nodes/regression-adjustment.md): 회귀를 조정과 비교의 도구로 읽기.
- [design-without-randomization](nodes/design-without-randomization.md): IV, LATE, matching, propensity score, doubly robust.
- [panel-time](nodes/panel-time.md): DID, fixed effects, synthetic control, RDD.
- [prediction-policy](nodes/prediction-policy.md): 예측 모델을 정책 결정 재료로 바꾸기.
- [heterogeneity](nodes/heterogeneity.md): ATE에서 CATE와 개인화로 이동하기.
- [orthogonal-ml](nodes/orthogonal-ml.md): nuisance model, orthogonalization, debiased ML.
- [modern-did-sdid](nodes/modern-did-sdid.md): heterogeneous DID 문제와 SDID.
- [inference](nodes/inference.md): 불확실성, 검정, 모델 평가, conformal inference.

## How To Use

새 번역 장을 만들 때는 원문 노트북을 바로 번역하지 않는다.

1. [coverage](coverage.md)에서 해당 장이 속한 노드를 찾는다.
2. [audience](audience.md)에서 학생 독자 기준을 확인한다.
3. 노드의 `Question`, `Reader State`, `Student Bridge`, `Rewrite Focus`를 먼저 읽는다.
4. 원문 장의 코드, 그림, 수식은 evidence로 남긴다.
5. 한국어 설명은 노드가 요구하는 판단 순서에 맞게 다시 쓴다.
6. [explanation-gaps](explanation-gaps.md)에서 해당 장의 선행 설명이 빠졌는지 확인한다.
7. 장 끝에는 다음 노드로 넘어가는 질문을 남긴다.

## Boundary

`causal-inference-for-the-brave-and-true/`는 upstream 원본이다. 이 그래프는 원본 폴더를 고치기 위한 문서가 아니다.

`causal-inference-for-the-brave-and-true-ko/`는 현재 삭제된 상태다. 한국어 강의노트를 다시 만들 때 이 이름으로 작업 폴더를 새로 만들고, 번역 품질 판단은 이 `graph/`를 기준으로 한다.
