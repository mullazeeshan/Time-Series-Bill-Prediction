# Time-Series-Bill-Prediction

Bill prediction (time series) for  n number of years. 
![1](https://user-images.githubusercontent.com/29397302/84136039-62417880-aa68-11ea-9358-a9e3a14a3fb7.gif)
![2](https://user-images.githubusercontent.com/29397302/84136143-843afb00-aa68-11ea-94f9-fb7fb616c25d.gif)
![3](https://user-images.githubusercontent.com/29397302/84136193-961c9e00-aa68-11ea-8d73-ad28f0367b18.gif)
![4](https://user-images.githubusercontent.com/29397302/84136371-d3812b80-aa68-11ea-92e9-dac503f5ab8f.gif)

“Time series models are used to forecast future events based on previous events that have been observed (and data collected) at regular time intervals.”

# variety of applications including:
- Weather forecasting- Earthquake prediction- Astronomy- Statistics- Mathematical finance- Econometrics- Pattern recognition- Signal processing- Control engineering

### This Repo Consists of :
A Univariate Prediction
It contains only 2 columns, one column is Date and the other column relates to the consumption percentage
Consumption From 1985 to 20166
![prj1](https://user-images.githubusercontent.com/29397302/84137168-eba57a80-aa69-11ea-96cb-8420dfe1ac38.png)

prediciton from 1985 to 2030
![prj2](https://user-images.githubusercontent.com/29397302/84137439-55258900-aa6a-11ea-9627-1a4b6692a559.png)

prediciton from 1985 to 2024
![prj3](https://user-images.githubusercontent.com/29397302/84137483-64a4d200-aa6a-11ea-9ca7-2126b7f819fe.png)

#Stages
Solving a time series problem is a little different as compared to a regular modeling task. A simple/basic journey of solving a time series problem can be demonstrated through the following processes. We will understand about tasks which one needs to perform in every stage. We will also look at the python implementation of each stage of our problem-solving journey.
Steps are –

<b>1. Visualizing time series</b>

In this step, we try to visualize the series. We try to identify all the underlying patterns related to the series like trend and seasonality. Do not worry about these terms right now, as we will discuss them during implementation. You can say that this is more a type of exploratory analysis of time series data.

<b>2. Stationarising time series</b>

A stationary time series is one whose statistical properties such as mean, variance, autocorrelation, etc. are all constant over time. Most statistical forecasting methods are based on the assumption that the time series can be rendered approximately stationary (i.e., “stationarised”) through the use of mathematical transformations. A stationarised series is relatively easy to predict: you simply predict that its statistical properties will be the same in the future as they have been in the past! Another reason for trying to stationarise a time series is to be able to obtain meaningful sample statistics such as means, variances, and correlations with other variables. Such statistics are useful as descriptors of future behavior only if the series is stationary. For example, if the series is consistently increasing over time, the sample mean and variance will grow with the size of the sample, and they will always underestimate the mean and variance in future periods. And if the mean and variance of a series are not well-defined, then neither are its correlations with other variables.

<b>3. Finding the best parameters for our model</b>

We need to find optimal parameters for forecasting models one’s we have a stationary series. These parameters come from the ACF and PACF plots. Hence, this stage is more about plotting above two graphs and extracting optimal model parameters based on them. Do not worry, we will cover on how to determine these parameters during the implementation part below!

<b>4. Fitting model</b>

Once we have our optimal model parameters, we can fit an ARIMA model to learn the pattern of the series. Always remember that time series algorithms work on stationary data only hence making a series stationary is an important aspect

<b>5. Predictions</b>

After fitting our model, we will be predicting the future in this stage. Since we are now familiar with a basic flow of solving a time series problem, let us get to the implementation.

### PS...

It contains only 2 columns, one column is Date and the other column relates to the consumption percentage.

It shows the consumption of electricity from 1985 till 2018. The goal is to predict electricity consumption for the next 6 years i.e. till 2024.
