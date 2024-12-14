# 2024 2학기 데이터 마이닝(이상민 교수님) Term Project

| **청년 치매걸린 아즈카반의 디멘터** 팀


## Introduction
AI-Hub [치매 고위험군 웨어러블 라이프로그](https://aihub.or.kr/aihubdata/data/view.do?currMenu=115&topMenu=100&aihubDataSe=realm&dataSetSn=226)데이터셋을 활용한
생체신호 기반 치매 분류 모델


## Data

- **Input** : **활동 데이터, 수면 데이터, 인지기능검사 데이터**
- **Label** : **CN : 정상인, MCI : 경도인지 장애 환자, Dem : 치매환자** 


## Code

### EDA
- **EDA_Whole_data.ipynb**, **EDA_Whole_data_2.ipynb**
    - 모든 데이터의 전반적인 EDA (길이 분포, Feature별 상관계수, 라벨별 Feature 분포 등)
    - 시계열 데이터에 대한 추가 분석

<br/>

- E**DA_Sleep_data.ipynb**
    - 수면 데이터속 유의미한 Feature 분석


<br/>

### Experiment

- **Experiment_BorderlineSMOTE.ipynb** *[Final Version]*
    - Borderline SMOTE 기법을 적용한 최고 성능 버전

<br/>

- **Experiment_Baseline.ipynb**, **Experiment_Baseline_2.ipynb**
    - 다양한 Baseline 모델의 성능 실험

<br/>

- **Experiment_Independent.ipynb**
    - 한 샘플 속 여러 데이터를 개별 샘플로써 독립적으로 간주하여 실험

<br/>

- **Experiment_Transformation.ipynb**
    - 데이터 분포의 왜도가 심한 Feature에 대한 log transformation을 적용하여 실험

<br/>

- **Experiment_DistantCentors.ipynb**
    - PCA상 거리를 넓히는 Feature를 후진 소거법으로 선택하여 실험

<br/>

- **Experiment_TimeSeries.ipynb**
    - 수면 데이터 속 시계열 특징을 사용하여 실험
