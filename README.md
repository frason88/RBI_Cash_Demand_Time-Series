# RBI_Cash_Demand_Time-Series

• Do ⭐ the repository if it helped you in anyway.

# Problem Statement:

ATMs filled with large amounts of cash may bring low transport/logistic cost but high freezing & high insurance cost. On the other hand, if banks do not have the proper mechanism to track the usage pattern, then frequent re-filling ATMs will reduce freezing and insurance cost but increase logistic cost. This is important, because it will allow the goverment to gain information about the cash flow in the economy, as well as analyze the cash demand required for each ATM banks.

# Data Collection:

Data is published on RBI website.

Source: https://www.rbi.org.in/Scripts/BS_PressReleaseDisplay.aspx?prid=49901

https://drive.google.com/file/d/1tu3iisCaOnwgc4Z510xypUGHQt80Vn-k/view?usp=sharing

# Comparing the model Analysis:

Model 1 is made using Moving Average. I have built other two models using SARIMAX. In the second model, I have manually selected the value of parameters p and q based on the ACF and PACF plot. And as the data is already stationary, there was no need to apply to the difference, and so the value of parameter d is 0. I have built a second model using auto arima to get the optimized value of p and q. The value of d is the same as model 2 that is ‘0’.
Model 1 RMSE : 330.95 Model 2 RMSE : 461.65 Model 3 RMSE : 331.14
If we compare the metrics for each model, we see that the RMSE for moving average and auto ARIMA model is approximately the same. However, the SARIMAX model considers both AR and MA properties. Therefore, we can conclude that model 3 is performing better compared to model 1 and model 2.

# Future work:

We can extend this model to forecast the cash demand for individual banks. Here, we have the data for ATM withdrawal across bank and so we can forecast the demand in total. However, if an individual bank forecasts the demand for their own ATMs, it can benefit them in following ways:

• Optimizing the logistic and insurance cost,

• Stabilizing the cash freeze,

• Improving the customer goodwill and so on.

# Refrences:
• https://www.geeksforgeeks.org/time-series-plot-or-line-plot-with-pandas/

• https://www.machinelearningplus.com/time-series/time-series-analysis-python/

• https://towardsdatascience.com/time-series-analysis-using-pandas-in-python-f726d87a97d8
