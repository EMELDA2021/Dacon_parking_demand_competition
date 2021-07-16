
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

