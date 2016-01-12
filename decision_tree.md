# Decision Tree
### Coding a Decision Tree
```
>>> from sklearn import tree

>>> clf = tree.DecisionTreeClassifier()
>>> clf = clf.fit(features_train, labels_train)
>>> clf.predict(features_test)
```

### Entropy
Controls how a Decision tree decides where to split the data<br>
**Definition** : measure of impurity in a bunch of examples<br>
Find the boundary that is as purity as possible

### Information Gain
information gain = entropy(parent) - weighted average * entropy(children)<br>
Decision tree algorithm : maximize information gain
