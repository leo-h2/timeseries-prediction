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
