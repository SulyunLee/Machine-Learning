# Naive Bayes
### Gaussian NB Example
```
>>> import numpy as np
>>> X = np.array([-1, -1], [-2, -1], [-3, -2], [1, 1], [2, 1], [3, 2]) // features
>>> Y = np.array([1, 1, 1, 2, 2, 2]) // labels
>>> from sklearn.naive_bayes import GaussianNB
>>> clf = GaussianNB() //classifier
>>> clf.fit(X, Y) // give training data and learn pattern
>>> print(clf.predict([[-0.8, -1]]))
```

### Accuracy of Naive Bayes
