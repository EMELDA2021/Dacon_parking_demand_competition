
# Dacon_parking_demand_competition
 - 평가산식 : MAE(Mean Absolute Error)
 - Public 평가 : 전체 Test 데이터 중 무작위 33% (50단지)
 - Private 평가 : 전체 Test 데이터 중 나머지 67% (100단지)

### 0714_전처리_hw
- PolynomialFeatures(degree=2)
- Ridge(alpha=0.5)
- MAE=127.55
 > 제출결과: 120.4316(248위)


### 0715_전처리_decisiontree
 - DecisionTreeClassifier(max_depth=35,random_state=0)
 - test_size : 0.3
 - train_acc : 0.8901258470474347
 - test_acc : 0.835214446952596
 - MAE=25.2
  > 제출결과: 205.03
![화면 캡처 2021-07-15 233924](https://user-images.githubusercontent.com/85726172/125807061-4e2974a2-b96a-4e52-bd68-6877c88bca1f.jpg)

### 0716_전처리_randaomforest
 - RandomForestClassifier(n_estimators=8, random_state=0)
 - 학습용 세트 정확도 : 0.999
 - 테스트 세트 정확도 : 0.971
 - MAE=4.3
  > 제출결과: 159.77
 ![화면 캡처 2021-07-16 205116](https://user-images.githubusercontent.com/85726172/125943281-3a614132-a087-4627-851c-70d003165690.jpg)

### 0717_전처리_ridge
 - PolynomialFeatures(degree=2, random_state=99)
 - 학습용 데이터 세트 점수 : 0.87
 - 테스트 데이터 세트 점수 : 0.85
 - model=Ridge(alpha=0.1)
 - MAE=113.98
  > 제출결과: 119.47(269위)
  
  cf)
  - train_test_split:test_size=0.3,random_state=99
  - PolynomialFeatures(degree=2, test_size=0.2, random_state=99)
  - 학습용 데이터 세트 점수 : 0.87
  - 테스트 데이터 세트 점수 : 0.84
  - model=Ridge(alpha=0.00001)
  - MAE=110.55
   > 제출결과: 119.87
  
  - 학습용 데이터 세트 점수 : 0.86
  - 테스트 데이터 세트 점수 : 0.86
  - MAE=112.29
   > 제출결과: 120.62

### 0719_전처리_gradient boosting
 - GradientBoostingRegressor(max_depth=3,random_state=0)
 - 학습(score) : 0.9549763891793135
 - 테스트(score) : 0.9491070691390533
 - MAE=72.43
  > 제출결과: 112.75(207위)

![grb](https://user-images.githubusercontent.com/85726172/126167908-975211d7-5e1c-4dd1-aa97-e89812ba0016.jpg)
