# Linear Regressions

* Regression analysis is one of the most important fields in statistics and machine learning. There are many regression methods available. Linear regression is one of them. Regression searches for relationships among variables.

* Linear regression is one of the fundamental statistical and machine learning techniques. Whether you want to do statistics, machine learning, or scientific computing, there are good chances that you’ll need it.

* Linear regression is probably one of the most important and widely used regression techniques. It’s among the simplest regression methods. One of its main advantages is the ease of interpreting results.

* The package `scikit-learn` : is a widely used Python library for machine learning, built on top of NumPy and some other packages. It provides the means for preprocessing data, reducing dimensionality, implementing regression, classification, clustering, and more. Like NumPy, scikit-learn is also open source.

### Scikit Learn

* Use a linear regression model and predict the Boston housing prices.

* Y = boston housing price(also called "targe" data in Python)

* X = all the other features(or independent variables)

* Drop price column and only use the parameters as the X values.

* from sklearn.linear_model import LinearRegression

* X = bos.drop('PRICE', axis = 1)

* Create the LinearRegression object: lm = LinearRegression()