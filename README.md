# Bike Sharing Demand

## Libraries
* numpy
* pandas
* matplotlib
* seaborn
* datetime
* calendar
* sklearn
  * RandomForestRegressor
  * preprocessing

## Columns
* datetime: hourly date + timestamp 
* season: 1 = spring, 2 = summer, 3 = fall, 4 = winter 
* holiday: whether the day is considered a holiday
* workingday: whether the day is neither a weekend nor holiday
* weather: 
  * 1: Clear, Few clouds, Partly cloudy, Partly cloudy
  * 2: Mist + Cloudy, Mist + Broken clouds, Mist + Few clouds, Mist
  * 3: Light Snow, Light Rain + Thunderstorm + Scattered clouds, Light Rain + Scattered clouds
  * 4: Heavy Rain + Ice Pallets + Thunderstorm + Mist, Snow + Fog 
* temp: temperature in Celsius
* atemp: "feels like" temperature in Celsius
* humidity: relative humidity 
* windspeed: wind speed
* casual: number of non-registered user rentals initiated
* registered: number of registered user rentals initiated
* count: number of total rentals

## Process
1. 匯入資料和套件
2. 處理時間格式
3. 異常值分析
4. 觀察參數分布情形
5. 將風速為0的資料進行補遺
6. 相關性分析
7. 透過取log使單車租借數量(count)分布接近Normal Distribution
8. 特徵選取
9. 使用Random forest進行預測
10. 訓練模型和預測結果
11. 提交結果

## Model Performance
Public Score: 0.42968
