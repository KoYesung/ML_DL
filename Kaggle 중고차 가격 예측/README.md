

<img src="https://capsule-render.vercel.app/api?type=waving&color=auto&height=200&section=header&text=중고차%가격%예측%모델&fontSize=90" />

## 프로젝트 개요

- 프로젝트 목적: kaggle에서 주최한 "**인도 중고차 예측하기**" 데이터를 바탕으로 인도 중고차 가격 예측하기
- 데이터: kaggle의 [인도 중고차 예측하기](https://www.kaggle.com/avikasliwal/used-cars-price-prediction) 데이터셋
- 팀원 총 6명 
- 사용한 언어
  - [![Python Badge](http://img.shields.io/badge/-Python%20-blue?style=flat-square&&logoColor=yellow&logo=python&link=https://www.python.org/)](https://www.python.org/) [![Numpy Badge](http://img.shields.io/badge/-Numpy%20-013243?style=flat-square&&logoColor=white&logo=numpy&link=https://numpy.org/)](https://numpy.org/) [![Pandas Badge](http://img.shields.io/badge/-Pandas%20-150458?style=flat-square&logoColor=white&logo=pandas&link=https://pandas.pydata.org/)](https://pandas.pydata.org/) [![Matplotlib Badge](http://img.shields.io/badge/-Matplotlib%20-2350A9?style=flat-square&logoColor=white&logo=matplotlib&link=https://matplotlib.org/)](https://matplotlib.org/) [![Seaborn Badge](http://img.shields.io/badge/-Seaborn%20-212E50?style=flat-square&logoColor=white&logo=seaborn&link=https://seaborn.pydata.org/)](https://seaborn.pydata.org/) [![Pyecharts Badge](http://img.shields.io/badge/-Pyecharts%20-34E0A1?style=flat-square&logoColor=black&logo=pyecharts&link=https://pyecharts.org/)](https://pyecharts.org/) [![Sklearn Badge](http://img.shields.io/badge/-Sklearn%20-F7931E?style=flat-square&logoColor=black&logo=scikit-learn&link=https://scikit-learn.org/stable/)](https://scikit-learn.org/stable/)


## 프로젝트 과정

<img src="https://user-images.githubusercontent.com/80456601/131045057-95de77e8-daa8-406d-a5f5-0f27627b95c2.png" width="80%" height="80%"/>

1. DB구조 파악 및 Column별 검토
2. 분석에 필요한 Column 추가, 제거 및 데이터 전처리 
3. EDA - 데이터 탐색 및 모델링에 필요한 Feature 파악
4. 모델 분석 및 구축
- LinearRegression 모델 구축
- RandomForest 모델 구축
- L1(Lasso)/L2(Rigde) 규제 적용
- ElasticNet, StandardElasticNet, PolyElasticNet 적용
- Stacking, Blending 적용 
5. 모델 검증

![image](https://github.com/KoYesung/ML_DL/assets/131944189/61c82f0e-0b60-40a0-8688-01879e4a9fd0)

6. 최종 결과
- 중고차 가격에 영향력 있는 feature Top10

   ![image](https://github.com/KoYesung/ML_DL/assets/131944189/f3c9ff60-2998-4a20-9654-5ec8dbe59cf6)



## 프로젝트 결과
![규제1](https://github.com/KoYesung/ML_DL/assets/131944189/e9d2ec1b-fbd4-411b-958e-5c2c01a4abf4)

- 사용한 모델 중 반복적인 모델링을 돌려 본 결과 RandomForestRegressor'이  정확도가 높아 채택
- 'LinearRegression'는 평균 제곱 오차: 26.47 ,'RandomForestRegressor'는 평균 제곱 오차: 6.764으로 'RandomForestRegressor'의 정확도가 높음.
- Random Forest의 MSE 값이 선형 회귀보다 더 낮은 이유는 Power를 제외한 나머지 데이터들이 선형이 아니기 때문이라 예측됨.
- Weighted Blending은 각 모델의 중요도에 따라 가중치를 조정하여 전체 예측 성능을 향상시킴.
- Weighted Blending은 다른 ensemble 모델과 달리 가중치를 조정하여 앙상블의 효과를 극대화 시킴.


#### [자세한 코드와 프로젝트 과정 여기를 클릭](https://github.com/KoYesung/ML_DL/blob/510b700da87a04f14b7be5fe600edcdda2cc4312/Kaggle%20%EC%A4%91%EA%B3%A0%EC%B0%A8%20%EA%B0%80%EA%B2%A9%20%EC%98%88%EC%B8%A1/%EC%A4%91%EA%B3%A0%EC%B0%A8%EA%B0%80%EA%B2%A9%EC%98%88%EC%B8%A1.ipynb)
#### [발표 PT 자료는 여기를 클릭](https://github.com/KoYesung/ML_DL/blob/510b700da87a04f14b7be5fe600edcdda2cc4312/Kaggle%20%EC%A4%91%EA%B3%A0%EC%B0%A8%20%EA%B0%80%EA%B2%A9%20%EC%98%88%EC%B8%A1/%EC%A4%91%EA%B3%A0%EC%B0%A8%EA%B0%80%EA%B2%A9%EC%98%88%EC%B8%A1_%EC%B5%9C%EC%A2%85%EB%B3%B8.pdf)
