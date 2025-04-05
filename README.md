# Time series analysis with ARIMA

Python example on how to use statsmodels.tsa.statespace.ARIMAX without dependent variables to forecast time series

it applies a grid-search on the order-space (p,d,q)x(P,D,Q) to find the model with the smallest Akaike Information Criterion (AIC)

# interesting stochastic functions/attributes

the result of a fit has the following attributes
- AIC: Akaike Information Criterion
- BIC: Bayes Information Criterion 

the result of a fint has the following functions
- plot_diagnostics():  analysis to show the forecast residuals behave like white noise 
    - plot of forecast residuals over time
    - histogram of forecast residuals with KDE-density and N(0,1)-density as reference
    - QQ-plot to compare quantiles of residuals with N(0,1)-quantiles 
    - Correlogram to visualise autocorrelation of residuals






