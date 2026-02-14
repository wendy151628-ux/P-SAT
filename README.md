# P-SAT
교내 데이터 분석 학회 P-SAT 활동 및 프로젝트 기록입니다.
통계 기반 분석부터 머신러닝, 시계열 모델링, 정책 시뮬레이션까지 수행한 프로젝트를 정리했습니다.

---

## 1. 노인의 사회적 고립 정책 효과 측정 모델 개발

보건복지부 노인실태조사 데이터를 기반으로 사회적 고립을 정량화하고, 정책 효과를 시뮬레이션 가능한 구조로 설계한 프로젝트입니다.

### Project Overview
- 사회적 고립을 복합 요인 기반 지수(Index)로 재정의
- 요인분석 기반 고립 지수 도출
- XGBoost, LightGBM 기반 모델링
- SHAP Value를 활용한 변수 영향력 해석
- R synthpop을 활용한 합성데이터 생성
- 정책 변수 변화에 따른 시뮬레이션 구조 구현

### Tech Stack
- Python: pandas, numpy, scipy, scikit-learn, xgboost, lightgbm, shap
- Statistical Methods: Chi-square Test, Factor Analysis, Cramer's V
- R: synthpop (CART 기반 합성데이터 생성)

### Key Contributions
- 범주형 변수 독립성 검정 기반 변수 선별
- 요인별 설명 분산을 반영한 고립지수 설계
- 클러스터링 기반 위험군 cut-off 설정
- SHAP 기반 설명 가능한 모델 구현
- 합성데이터 기반 정책 효과 분석 구조 설계

### Skills Gained
- 정책·사회 데이터를 정량 지표로 구조화하는 능력
- 통계 분석과 머신러닝 결합 설계 역량
- 설명 가능한 AI 기반 해석 경험
- End-to-End 분석 수행 경험

---

## 2. 미국 도소매 시장 동향 분석 및 중소기업 수출 기회 발굴 모델

미국 수입 데이터, NAICS 산업 코드, 거시경제 지표를 활용하여 산업별 시장 진입 타이밍과 위험 지수를 산출한 프로젝트입니다.

### Project Overview
- 미국 총 수입액 대비 對한국 수입액 기반 시장 경쟁력 지표 설계
- BCG Matrix 논리를 확장한 시장 진입 판단 구조 구축
- 시계열 분해 및 파생변수 설계
- PCA 기반 기업 위험 지수 산출
- Prophet 기반 시계열 결측치 보간
- 산업·관세·거시경제 지표 통합 위험 모델 구축

### Tech Stack
- Python: pandas, numpy, statsmodels, scikit-learn(PCA), prophet
- Time Series: Additive Decomposition, Polynomial Regression
- Scaling: MinMax Scaling
- Multivariate Model: Dynamic Factor Model

### Key Contributions
- HS Code → NAICS 코드 매핑을 통한 산업 단위 통합
- 3차 회귀 기반 추세 증감 지표 설계
- 1차 미분 분산 기반 변동성 지표 설계
- PCA 기반 가중치 산출 및 기업 지수 설계
- 관세(AHS Weighted Average) 반영 위험 지수 설계

### Skills Gained
- 산업·무역 데이터 기반 시장 분석 역량
- 시계열 데이터 구조적 신호 추출 능력
- 파생변수 설계 및 지수화 경험
- 복수 지표 통합 의사결정 모델 설계 경험

---

## 3. 시계열 다중 분류 해커톤

0~499 시계열 데이터 기반 다중 분류 문제 해결 프로젝트입니다.

### Problem Definition
- 587,880개 결측치 존재
- Label 0/1/2 다중 분류
- 클래스 불균형 존재
- 범주형 + 시계열 혼합 데이터

### Tech Stack
- Python: pandas, numpy, scipy, scikit-learn
- Models: XGBoost, LightGBM, KNN, Logistic Regression, CNN
- Imbalance Handling: SMOTE, Random Over/Under Sampling
- Missing Value Handling: FFT 기반 보간

### Key Contributions
- 결측치 위치 분석 및 연속 구간 패턴 확인
- 선형·스플라인·FFT 비교 후 FFT 채택
- 클래스 불균형 해결 전략 실험
- Scaling 적용 시 성능 저하 분석
- 트리 기반 모델에서 안정적 성능 확보

### Skills Gained
- 시계열 결측치 복원 설계 역량
- 주파수 도메인 기반 신호 처리 경험
- 다양한 모델 비교 및 실험 설계 능력
- 데이터 특성 기반 전처리 전략 수립 경험

---

## Core Competencies
- End-to-End 데이터 분석 수행 능력
- 통계 기반 검정 및 머신러닝 모델링 역량
- 시계열·정책·산업 데이터 분석 경험
- 지수(Index) 설계 및 의사결정 모델 구조화 능력
- 설명 가능한 모델 기반 인사이트 도출 역량
