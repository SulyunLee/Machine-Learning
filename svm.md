# SVM
### SVM in sklearn
```
>>> from sklearn import svm
>>> X = [[0, 0], [1, 1]] # training feature
>>> y = [0, 1]  # training label
>>> clf = svm.SVC()
>>> clf.fit(X, y)
>>> clf.predict([[2., 2.]])
```

### Kernel Choices
```
from sklearn.svm import SVC
clf = SVC(kernel="linear")
clf.fit(features_train, labels_train)
pred = clf.predict(features_test)

prettyPicture(clf, features_test, label_test)
plt.show()

from sklearn.metrics import accuracy_score
acc = accuracy_score(pred, labels_test)
print "accuracy: ", acc
```

### Parameters in Machine learning
* kernel
* C : control tradeoff between smooth decision boundary and classifying training points correctly<br>
Large C means you expect a more training points correct
* gamma
