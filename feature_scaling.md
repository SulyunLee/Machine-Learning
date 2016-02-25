# Feature Scaling
Feature scaling: usually [0,1]
Rescale into new range for more sensible results.

### Features scaling formula
<img src="feature_scaling1.jpg">
x' : new(rescaled) feature
0 <= x' <= 1

### Min/Max Scaler in sklearn
```
>>> from sklearn.preprocessing import MinMaxScaler
>>> import numpy
>>> weights = numpy.array([[115.0], [140.0], [175.0]])
>>> scaler = MinMaxScaler()
>>> rescaled_weight = scaler.fit_transform(weights)
>>> rescaled_weight
### Prints out the rescaled weight in list.
```
