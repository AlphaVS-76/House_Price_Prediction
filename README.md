# House Price Prediction Documentation

This Repository contains the source code for Predicting House Prices using Linear Regression Algorithm(Supervised Learning).

## Introduction:

Accurately estimating the value of real estate is an important problem for many
stakeholders including house owners, house buyers, agents, creditors, and investors. It is also a difficult one. Though it is common knowledge that factors
such as the size, number of rooms and location affect the price, there are many
other things at play. Additionally, prices are sensitive to changes in market
demand and the peculiarities of each situation, such as when a property needs
to be urgently sold. The sales price of a property can be predicted in various ways, but is often
based on regression techniques. All regression techniques essentially involve
one or more predictor variables as input and a single target variable as output.

## Tool Prerequisites:
1. Pandas
2. Matplotlib
3. Scikit-Learn (Linear regression)

## Linear Regression:

[Linear regression](https://en.wikipedia.org/wiki/Linear_regression) is a linear approach for modelling the relationship between a Dependant variable(Output) and an Independant variable(Input). Different techniques can be used to prepare or train the linear regression equation from data, the most common of which is called [Ordinary Least Squares](https://en.wikipedia.org/wiki/Ordinary_least_squares#:~:text=In%20statistics%2C%20ordinary%20least%20squares,in%20a%20linear%20regression%20model.&text=Under%20these%20conditions%2C%20the%20method,the%20errors%20have%20finite%20variances.).

## Steps to create the Model:
1. Import the required libraries and modules,
 ```
import pandas as pd
from sklearn.linear_model import LinearRegression
import matplotlib.pyplot as plt
```
2. Create a dataframe of the given dataset using Pandas.
3. Define Inputs(Independant variables) and Outputs(Dependant variables) as `x` and `y`.
4. Use the `LinearRegression()` function in the variable `model` and Fit the data using the `model.fit()` function.
5. Find the predicted values using the `model.predict()` function and assign it to `y_pred`. 

### Validation:
Validate the predicted values by taking a random value for prediction,
```
model.predict([[2500]])
```
### Visualization:
Visualize the plot by using `plt.plot()` function,
```
plt.ylabel("PRICE IN LAKH")
plt.xlabel("AREA IN SQFT")
plt.plot(x,y_pred)
```
