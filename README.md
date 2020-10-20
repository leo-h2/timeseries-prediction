# timeseries-prediction
coursera sequences, time series and prediction

week 1

time series 의 종류   
: 주기성을 갖는 경우와 비 주기성 신호로 구분 가능

# introduction to tiem series 
auto corrrelation (자기 상관) : 시간 또는 공간적으로 연속되는 일련의 관측치들간에 존재하는 상관 관계

# Fiexd partitioning    
train / valid / test set    

# Metrcis for evaluating performance   

erros = forecasts - actual   
mse = np.square(errors).mean()   
rmse = np.sqrt(mse)   
mae = np.abs(errors).mean()    
mape = np.abs(erros/x_valid).mean()   

keras.metrics.mean_absolute_error(x_valid, naive_forecast).numpy()   

# Moviing Average and differing
Moving average 를 이용하여 노이즈를 제거

# Trailing versus centered windows   

# forecasting 
참조 코드
split data

split_time = 1000   
time_train = time[:split_time]   
x_train = series[:split_time]    % 0 에서 부터 split_time 까지 데이터를 train 데이터로 활용     
time_valid = time[split_time:]   % split_time 이후 데이터로 정해 짐
x_valid = series[split_time:]   




