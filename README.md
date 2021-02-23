# 개요
* 일정기간동안 측정된 주식 데이터셋이 주어집니다.
* Train set과 Test set이 주어집니다.
* Train set에 대해서 학습을 진행하고, Test Set을 통한 prediction을 만드는 것이 목표입니다.

# 데이터 설명
  
*Input data*  
  
* 데이터셋의 각 column은 날짜정보와 종목정보, 그리고 Feature set으로 이루어져 있습니다. Feature set은 blur 처리되어 있습니다. 
* Feature는 각 종목들의 유의미하다고 판단되는 데이터 값으로 이루어져 있습니다.

*Target data*
  
* Train set에 대해서는 정답 데이터 2개가 주어지고, Test set에 대해서는 정답이 주어지지 않습니다. 정답 데이터들은 각 샘플 시간 기준으로 다음 단위시간(T) 수익률로 만들어집니다.
* 정답 데이터1: 단위시간(T) 수익률 (train_target.csv) → Regression
* 정답 데이터2: 특정 한 시점에서 종목들의 단위 시간 수익률(정답데이터 1)을 5분위로 나누어 분류한 Target (train_target2.csv) → Classification

