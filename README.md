# Tunisian_Stock_Index_Forecasting
Building a forecasting model to forescast stock index in Tunisia (TUNINDEX).

## step1:Data collection and preparation
the data is composed of text files dowloaded from http://www.bvmt.com.tn/en-gb/content/historical-data
I scraped and converted each of these text files to csv files , check out the code https://github.com/FirasMezghi/Tunisian_Stock_Index_Forecasting/blob/main/stock.ipynb,
and then merged all the csv files in on ,check out the code https://github.com/FirasMezghi/Tunisian_Stock_Index_Forecasting/blob/main/create_stock_data.ipynb

## step2: build an arima model
although an arima model doen't fit to these kind of problems , because linear models are to simple to predict stock indexes, but it is good to give it a go.
check out the modeling https://github.com/FirasMezghi/Tunisian_Stock_Index_Forecasting/blob/main/stock_forecat_arima.ipynb
the results :
![image](https://user-images.githubusercontent.com/99277115/162591833-b9315e14-e3b9-4b51-acfc-40aaa421f10e.png)
we can see that this model doesn't show promising results 

## srep3: build an lstm model:
check out https://github.com/FirasMezghi/Tunisian_Stock_Index_Forecasting/blob/main/stock_forecast_lstm.ipynb
results :
![image](https://user-images.githubusercontent.com/99277115/162591910-5fe60fe1-b93f-460f-af72-e00bea038c9d.png)
we can see that we a better results(the blue is the entire data ,the orange is the predicted training data, the green is the predicted validation data and the red is the predicted test data)
