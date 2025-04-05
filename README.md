# Time series analysis with ARIMA

Python example on how to use statsmodels.tsa.statespace.ARIMAX without dependent variables to forecast time series

The example applies a grid-search on the order-space (p,d,q)x(P,D,Q) to find the model with the smallest Akaike Information Criterion (AIC)

The model residuals are analysed to see if they adhere white noise properties

The model data, predictions and forecasts are plotted with confidence intervals

# Interesting stochastic functions/attributes

The result of a fit has the following attributes & functions
- AIC: Akaike Information Criterion
- BIC: Bayes Information Criterion 
- plot_diagnostics():  analysis to show the forecast residuals behave like white noise 
    - plot of forecast residuals over time to show there is no trend
    - histogram of forecast residuals with KDE-density and N(0,1)-density as reference
    - QQ-plot to compare quantiles of forecast residuals with N(0,1)-quantiles 
    - Correlogram to visualise autocorrelation of forecast residuals
- prediction(): makes predictions of the training data (model has seen the data)
    - 1-step ahead prediction
    - dynamic prediciton
- forecast(): makes a forecast complementary to the training data (model has't seen the data)

The result of the prediction and forecast functions has the following attribute & function
- predicted_mean: mean of the prediction/forecast
- conf_int(): confidence interval of the prediction/forecast




