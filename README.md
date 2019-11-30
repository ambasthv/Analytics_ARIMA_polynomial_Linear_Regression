# Analytics_ARIMA_polynomial_Linear_Regression
Auto-Regressive Integrated Moving Average

# What ARIMA stands for
• A series which needs to be differenced to be made stationary is an “integrated” (I) series
• Lags of the stationarized series are called “autoregressive” (AR) terms
• Lags of the forecast errors are called “moving average” (MA) terms
• We’ve already studied these time series tools separately: differencing, moving averages, lagged values of the dependent variable in regression
#ARIMA models put it all together
• Generalized random walk models fine-tuned to eliminate all residual autocorrelation
• Generalized exponential smoothing models that can incorporate long-term trends and seasonality
• Stationarized regression models that use lags of the dependent variables and/or lags of the forecast errors as regressors
• The most general class of forecasting models for time series that can be stationarized* by transformations such as differencing, logging, and or deflating

#Polynomial Regression Models

The polynomial models can be used in those situations where the relationship between study and
explanatory variables is curvilinear. Sometimes a nonlinear relationship in a small range of explanatory
variable can also be modeled by polynomials.

# Considerations in fitting polynomial in one variable
Some of the considerations in fitting polynomial model are as follows:

#1. Order of the model

The order of the polynomial model is kept as low as possible. Some transformations can be used to keep
the model to be of first order. If this is not satisfactory, then second order polynomial is tried. Arbitrary
fitting of higher order polynomials can be a serious abuse of regression analysis. A model which is
consistent with the knowledge of data and its environment should be taken into account. It is always
possible for a polynomial of order ( 1) n − to pass through n points so that a polynomial of sufficiently
high degree can always be found that provides a “good” fit to the data. Such models neither enhance the
understanding of the unknown function nor be a good predictor.

#2. Model building strategy:

A good strategy should be used to choose the order of an approximate polynomial.
One possible approach is to successively fit the models in increasing order and test the significance of
regression coefficients at each step of model fitting. Keep the order increasing until t -test for the highest
order term is nonsignificant. This is called as forward selection procedure.
Another approach is to fit the appropriate highest order model and then delete terms one at a time
starting with highest order. This is continued until the highest order remaining term has a significant t -
statistic. This is called as backward elimination procedure.
The forward selection and backward elimination procedures does not necessarily lead to same model. The
first and second order polynomials are mostly used in practice.

# 3. Extrapolation:
One has to be very cautions in extrapolation with polynomial models. The curvatures in the region of data
and region of extrapolation can be different. For example, in the following figure, the trend of data in the
region of original data is increasing but it is decreasing in the region of extrapolation. So predicted
response will not be based on the true behaviour of the data. 
