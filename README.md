# 팀 abc
## 1) 본 연구는 제2회 ETRI 휴먼이해 인공지능 논문경진대회 참가한 연구입니다.

### 2) 연구 내용은 수집가능한 라이프로그 데이터를 활용하여 수면관련 항목 (수면 만족도, 수면의 질, 악몽 여부, 수면 이후 주관적 신체상태, 수면 이후 주관적 감정상태)의 예측 모델 성능 평가를 하였습니다.

### 3) 주요 피처의 데이터 전처리는 

> (1) 수면 전 1시간 이내의 e4Bvp, e4Eda, e4Hr, e4Temp 평균 값 추출 (e4_mean.ipynb)

> (2) GPS 기반 운동거리 추출 (final_gps_data_preprocessing.ipynb)

> (3) Google API 기반 운동 시간 추출 (data_preprocessing_activity_2018.ipynb, data_preprocessing_activity_2019.ipynb, data_preprocessing_activity_2020.ipynb)

> 로 이루어졌으며, 그 외 기본 나이 성별 등 인구학적 변수와 설문 기반 건강행태 변수가 input feature 로 사용되었습니다.

> (4) 전처리된 데이터셋은 data 폴더에 업로드되어있으며, data_merge.ipynb 파일에서 merge 되었습니다.

### 4) 하루에 2번 이상 수면기록이 있는 경우, 더 긴 수면기록으로 사용되었으며, single 및 double ensemble method을 통해 라이프로그 데이터 기반 수면관련 예측의 성능을 평가하였습니다.

### 5) ensemble method 는 Logistic regression, XGBoost, Decision tree, Light GBM, RandomForest 모델이 classifier 로 사용되었으며, 각 모델의 성능과 ensmeble method의 성능을 비교하였습니다.

##### * 구체적 연구 방법 및 결과는 KCC 2023 : 한국컴퓨터종합학술대회 초록집을 참고하시면 좋을 것 같습니다. 

##### * raw data는 ETRI 사이트에서 협약서 제출 후에 사용할 수 있습니다. (https://nanum.etri.re.kr/share/schung1/ETRILifelogDataset2020?lang=ko_KR)

##### * raw data에서 feature extraction 전 필요한 중복 값 제거, 데이터셋 분할 작업은 sas 에서 이루어졌습니다.

