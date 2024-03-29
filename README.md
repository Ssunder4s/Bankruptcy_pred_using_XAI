# XAI를 활용한 중소기업 부도예측 연구

## 1. 문제상황
### 정확한 부도 예측을 위한 머신러닝의 활용성이 높아지고 있음
- 전통적 통계기법은 여러 가정들을 충족 해야 된다는 한계점 존재
- 머신러닝과 딥러닝 기법은 비모수적 방법론이므로 여러 가정을 충족할 필요가 없음
- 1980 년대 이후 인공신경망, SVM 등 머신러닝 모델이 전통적 통계기법 대비 우수한 예측력을 보임

### 데이터 불균형 문제
- 기업부도 데이터는 건전기업과 부도기업의 비율이 1000:1 까지 나는 전형적인 불균형 데이터임
- 전통적 통계기법의 경우 여러 가정을 적용하는 과정에서 데이터 불균형이 해소되지만 ML/DL의 경우는 그렇지 않음

### 모델 투명성 문제
- 정확도 향상을 위해 복잡한 모델을 설계한 결과, 모델의 결과 값이 복잡하여 해석할 수 없는 문제가 발생
- 최근 AI 윤리 이슈로 인해 모델의 투명성 확보에 대한 규제강화 및 법제화가 진행 중임

## 2. 필요성
- (정부 차원) 과학적이고 체계적인 부도예측 시스템을 도입하여 중소기업의 연쇄 도산을 막을 필요성이 있음
- (금융 기관) 중소기업은 재무정보의 신뢰성이 낮고 비대칭성이 높으므로 머신러닝을 통해 이를 보완 할 수 있는 방법론 도입이 필요함
- (거래 기업) 사업 리스크 관리를 위해 부도 가능성이 높은 기업과의 거래를 회피할 필요성이 존재함

## 3. 데이터셋
- 중소기업현황정보시스템 재무 데이터
- 국세청 사업자등록상태조회 활용

## 4. 결과 및 액션
- 다양한 머신러닝 모델을 비교
- Stacking을 통해 모델 성능을 극대화 하였음
- PDP(부분의존도)를 활용하여 XAI 분석을 수행함
- 매출구조, 자본구조, 부채-자산구조에 따른 종합적 제언을 제시함

## 5. 분석 내용
- 데이터 수집(셀레니움을 활용한 동적스크레이핑)
- Feature Engineering(파생변수생성, 이상치처리, Fermutation Importance - Feature Selection)
- 하이퍼파라미터 튜닝(Bayesian Optimization)
- 모델 앙상블(Stacking)
- XAI (PDP 활용)
