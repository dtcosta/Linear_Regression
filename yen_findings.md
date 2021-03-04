# A Yen For The Future

## Background
The financial departments of large companies often deal with foreign currency transactions while doing international business. As a result, they are always looking for anything that can help them better understand the future direction and risk of various currencies. Hedge funds, too, are keenly interested in anything that will give them a consistent edge in predicting currency movements.
In this Analysis, I will test my data using the ARMA, ARIMA, and GARCH models in order to predict future movements in the value of the Japanese yen versus the U.S. dollar.


## Time-Series Forecasting

## Questions
1. Based on your time series analysis, would you buy the yen now?
2. Is the risk of the yen expected to increase or decrease?
3. Based on the model evaluation, would you feel confident in using these models for trading?

## Steps Taken:
1. Decomposition using a Hodrick-Prescott Filter (Decompose the Settle price into trend and noise).
2. Forecasting Returns using an ARMA Model.
3. Forecasting the Settle Price using an ARIMA Model.
4. Forecasting Volatility with GARCH.

## Conclusion
Based on the time series analysis, I would not feel confident using this data to purchase Yen. My reasoning is because both the ARIMA and ARMA model have a P value greater than 0.05; therefore the model resulsts are not significant. 

However, the GARCH model is significant (P Value on Omega and Alpha1 < 0.05) and predicts short-term volatility will increase. Depending on your risk tolerance an increase in volatility might be perceived as an increase in risk. If you are a riskier investor short term volatility of currencies might lead to an investment opportunity. 

I would not feel comfortable using these models to trade (succesfully) solely on the results of these models and would continue to train models in search for significant results.

## Linear Regression Forecasting

### Question
1. Does this model perform better or worse on out-of-sample data compared to in-sample data?

### Steps taken:
1. Data Preparation (Creating Returns and Lagged Returns and splitting the data into training and testing data)
2. Fitting a Linear Regression Model.
3. Making predictions using the testing data.
4. Out-of-sample performance.
5. In-sample performance.

## Conclusion
Summary of results:
Out-of-Sample Root Mean Squared Error (RMSE): 0.4154832784856737
In-sample Root Mean Squared Error (RMSE): 0.5963660785073426

Conclusion:
The out-of-sample performed slightly better than the in-sample.
