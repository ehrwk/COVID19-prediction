# 코로나 예측모델 만들기
19101252 윤희서

### ARIMA 모델과 Prophet 모델을 이용해서 코로나바이러스19 확진자추세를 예측해보고자 합니다.

## ARIMA 모델
- 확진자는 최근 3달을 가져와 표시해줍니다.
- p value 0.05 기준으로 판단하여 모델의 MA(1)은 유효하다고 판단, 최근 14일을 기준으로 예측모델을 만들었습니다.
- <img src = "https://github.com/ehrwk/COVID19-prediction/blob/main/Arima.png" width = "450px"></img>

## Prophet 모델
- 확진자는 2020년 1월 22일부터 최근일자까지 가져와 표시합니다.
- 데이터의 크기가 2년을 조금 안되므로, 일주일과 일일에 대하여 예측을 반영하였습니다.

## Dataset
- 코로나바이러스19로 인한 확진자, 사망자, 데이터셋은 매일 업데이트 되며, 출처는 다음과 같습니다. 

- [Number of Confirmed Cases (Daily Updated)](https://raw.githubusercontent.com/datasets/covid-19/master/data/time-series-19-covid-combined.csv)

## 참고자료
- https://dacon.io/codeshare/2570
- https://github.com/kairess/corona-virus-prediction/blob/master/corona19_confirmed_prediction.ipynb
