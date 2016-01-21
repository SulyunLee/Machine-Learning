# Regressions
### Continuous vs Discrete
**age**: Continuous<br>
**weather**: discrete<br>
**person wrote email**: discrete (order doesn't exist)<br>
**phone**: discrete<br>
**income level**: Continuous (order)<br>
<hr>

### Linear Regression Coding
```
>>> from sklearn import linear_model
>>> clf = linear_model.LinearRegression()
>>> clf.fit([[0,0], [1,1], [2,2]] [0, 1, 2])
>>> clf.predict(test_x)
>>> reg.coef_  # return coefficient(slope)
>>> reg.intercept_  # return intercept
>>> reg.score(x_test, y_test)  # return R-squared score of test sets
```
<hr>

### Linear Regression Errors
error = actual y - predicted y<br>
Minimizing the sum of squared errors:<br>
minimizes the sum of (actual-predicted)^2 of all training points<br>
##### Several algorithms
* ordinary least squares(OLS): used in sklearn linear regression
* gradient descent
<hr>

Minimizing the sum of squared errors will make implementation much easier.<br>

### Problem with SSE
If you add more data, the sum of the squared error(SSE) gets go up. Larger SSE means worse fit
<hr>

### R Squared Metric for Regression
R squared answers the question, "how much of my change in the output(y) is explained by the change in my input(x)"
0.0<r^2<1.0
r^2 = 0.0: Line isn't doing a good job of capturing trend in data.<br>
r^2 = 1.0: Line does a good job of describing relationship between input and output.<br>

### R Squared in sklearn
```
>>> from sklearn.linear_model import LinearRegression
>>> reg = LinearRegression()
>>> reg.fit(ages, net_worths)
>>> reg.predict([27])
>>> reg.score(ages, net_worths)
>>> reg.coef_
>>> reg.intercept_
```
