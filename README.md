해당 데이터 분석은 **매출 향상을 위한 마케팅을 수립하기 위해, 성별에 따른 구매패턴을 분석해본다는 가정**을 두고 진행한 **Kaggle 데이터 활용 프로젝트**입니다.
데이터 분석의 목적, 가설을 가정하여 분석 프로젝트를 진행해보았습니다.


![family-2923690_1920](https://user-images.githubusercontent.com/79372217/115143798-6248d680-a084-11eb-9359-92e2201b14b1.jpg)



**미국 AC SuperMarket(가명)은 3개의 분점(A, B, C)이 있는 작은 회사입니다.
본사는 매출 향상 위한 마케팅을 수립하기 위해, 성별에 따른 구매패턴을 분석해보고자 합니다.**
 

**문제**

최근 데이터에는 개인정보 이슈로 성별 데이터를 취합하지 않습니다. 따라서, 구매 이력이 기입됐을 때 성별을 자동 예측해야 합니다.

**목표**

구매 이력 데이터를 보고, 이들의 성별을 자동 분류하는 AI 모델을 만들어야 합니다. 이를 통해 BI를 제공합니다.

**문제해결 방법**

분류 모델을 활용한 기계학습(ML)

**주어진 정보**

고객 구매 데이터

 
------------------------------


**Features 설명**

* Gender(Target) : 성별. Target.
* Unnamed: 0_x : 인덱스
* Invoice ID : 구매내역 식별 위한 유니크 ID
* Branch : 지점명 (A,B,C 지점)
* City : 지역
* Customer type : 고객 유형 (회원, 비회원)
* Product line : 총 6개의 상품군으로 분류됨
* Unit price : 제품 1개 당 가격
* Quantity : 구매한 제품 수량
* Tax 5% : 세금 5% 금액
* Total : 구매한 제품 총액
* Date : 날짜
* Time : 시간
* Payment : 지불 유형 (카드, 현금, E월렛)
* cogs : 매출원가
* gross margin percentage : 매출 이익율
* income : 수입
* Rating : 고객 등급


-----------------------


[01 [EDA] Exploratory Data Analysis](https://github.com/mynameis-sohee/Customer-Gender-Prediction/commit/8d28b9a12a455ed02b6d6ec2550587bec7990ad0)

데이터의 분포는 어떤지, 결측치는 존재하는지 등 데이터의 EDA를 살펴보는 단계입니다.

&nbsp;

[02 [전처리(1)] Data Preprocessing 1](https://github.com/mynameis-sohee/Customer-Gender-Prediction/blob/main/02_%5B%EC%A0%84%EC%B2%98%EB%A6%AC(1)%5D_Data_Preprocessing_1.ipynb)

데이터 전처리 첫 단계입니다. 결측치 삭제, 인코딩, 데이터셋 분할 등 데이터 전처리의 전반적 작업을 진행하는 단계입니다.

&nbsp;


[03 [모델링(1)&전처리(2)] Modeling_1 & Data Preprocessing_2](https://github.com/mynameis-sohee/Customer-Gender-Prediction/commit/9ec07b7b06932c533e27da447767e0d1bf3b4589)

데이터 전처리 두 번째 단계이자, 모델링 첫 번째 단계입니다. 전처리의 경우, 특성중요도를 살펴보고 중요도가 낮은 Features에 대해 Feature Engineering 등의 추가 전처리를 수행합니다. 그후, 최적화 모델을 선택하여 모델링을 수행합니다. 

&nbsp;


[04 [모델링(2)] Modeling_PDP, SHAP](https://github.com/mynameis-sohee/Customer-Gender-Prediction/commit/dae9436b36e5edb830c6c1c2befe465e6039733e)

PDP, SHAP을 추가로 수행하여 모델링 이후의 과정을 분석해봅니다. 모델링 결과값이 어떻게 산출된 것인지 확인할 수 있습니다.

&nbsp;
