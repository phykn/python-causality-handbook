# Audience

이 그래프의 한국어 강의노트는 중/고등학생이 읽을 수 있어야 한다.

목표는 내용을 낮추는 것이 아니다. 어려운 개념을 숨기지 않고, 학생이 판단 순서를 잃지 않게 설명한다.

## Assumed Reader

독자는 다음을 알고 있을 수 있다.

- 평균, 비율, 그래프 읽기.
- 간단한 일차식.
- 학교, 병원, 광고, 쿠폰, 시험, 약 복용 같은 생활 사례.

독자는 다음을 이미 안다고 가정하지 않는다.

- 회귀분석.
- 통계적 검정과 p-value.
- 행렬, 미적분, 최적화.
- 머신러닝 모델 구조.
- 영어 약어의 의미.

## Explanation Ladder

새 개념은 항상 이 순서로 설명한다.

1. `Situation`: 생활 속 상황을 놓는다.
2. `Question`: 무엇을 알고 싶은지 한 문장으로 묻는다.
3. `Bad Shortcut`: 왜 쉬운 비교가 틀릴 수 있는지 보인다.
4. `Fair Comparison`: 어떤 비교가 더 공정한지 말한다.
5. `Method Name`: 그 비교를 만드는 방법 이름을 붙인다.
6. `Math or Code`: 이미 말한 비교를 수식이나 코드로 확인한다.
7. `Limit`: 그래도 남는 의심을 말한다.

## Student-Friendly Style

- 한 문단에는 새 용어를 하나만 넣는다.
- 영어 약어는 처음에 풀어 쓴다.
- 공식은 먼저 말로 설명하고, 그 다음에 쓴다.
- 코드 셀 앞에는 코드가 확인하려는 질문을 한 문장으로 둔다.
- 그래프와 그림은 "무엇을 먼저 보고, 무엇을 비교해야 하는지"를 안내한다.
- 장 끝에는 학생이 스스로 답할 수 있는 확인 질문을 남긴다.

## Good Explanation Pattern

나쁜 설명:

- `DID는 parallel trends assumption 아래 ATT를 식별한다.`

좋은 설명:

- `광고판을 설치한 도시의 매출이 늘었다고 해서 광고판 때문이라고 바로 말할 수는 없다. 광고판이 없는 도시도 같은 시기에 매출이 늘었을 수 있다. 그래서 우리는 "광고판이 있는 도시와 없는 도시의 차이"가 설치 전후에 어떻게 바뀌었는지 비교한다. 이 비교가 믿을 만하려면, 광고판이 없었다면 두 도시가 비슷한 방향으로 변했을 것이라는 가정이 필요하다. 이것을 parallel trends라고 부른다.`

## Terms That Need A Bridge

다음 용어는 반드시 생활 사례나 작은 숫자 예시 뒤에 등장해야 한다.

- treatment, outcome, counterfactual, potential outcome.
- bias, confounding, selection, collider, control.
- standard error, confidence interval, p-value.
- regression, coefficient, dummy variable, residual.
- instrumental variable, first stage, reduced form, LATE.
- matching, propensity score, positivity, doubly robust.
- parallel trends, fixed effects, synthetic control, cutoff, RDD.
- prediction, policy, ATE, CATE, uplift, sensitivity.
- nuisance model, orthogonalization, debiased ML, cross-fitting.

## Review Questions

각 장을 검토할 때 다음 질문에 답한다.

1. 중학생이 첫 사례를 읽고 "무엇을 비교하는지" 말할 수 있는가?
2. 고등학생이 수식 없이도 방법의 목적을 설명할 수 있는가?
3. 새 용어가 나오기 전에 그 용어가 필요한 상황이 보이는가?
4. 코드와 수식이 설명을 대체하지 않고 설명을 확인하는가?
5. 장 끝에서 학생이 다음 장의 질문을 예상할 수 있는가?
