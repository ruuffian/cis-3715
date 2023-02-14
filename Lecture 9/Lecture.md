February 14th, 2023

Summary of What I think I missed:
- Build Model
	- $f(x_i) = w_0 + w_1x_{i,1} + w_2x_{i,2} \dots w_dx_{i, d}$ 
- Split the data set, about 70/30 training and testing.
- Gradient Descent
	- $x_{t+1} = x_t - n \nabla f(x_t)$ 
	- Basically move in the opposite direction of the gradient to minimize the loss function ($f(x_t)$).
	- Linear Regression: $min_w ||y - Xw||^2$ has gradient $-2X^T(y-Xw)$, so gradient descent looks like this:
		- $w_{t+1} = w_t - n(2X^T(Xw_t - y))$
- Overfitting: Errors on training data is very good, but errors on new data points are very large.
	- How to avoid? add a regularization term - basically a constant to stop overfitting
	- Ridge Regression: use l-2 norm
		- $min_w \frac{1}{n} ||y-Xw||^2_2 + \lambda||w||^2_2$ 
	- Lasso: use l-1 norm
		- $min_w \frac{1}{n} ||y - Xw||_1 + \lambda||w||_1$
	- Difference: Lasso Model will always have a sparse vector, whereas ridge regression will have a vector of differences

### Classification

*Binary Classification*: Only two classes, 0-1, fraud-not fraud etc.
A classical example of a binary classification problem is detecting if an email is spam or not.
*Multi-Class Classification*: Many classes to classify.

##### Binary Classification
- Learn a classifier to seperate positive samples from negative samples
	- A good practice to get into is to use 0 and 1 as labels

Given n-samples: $\{(x_1, y_1), (x_2, y_2), \dots , (x_n, y_n)\}$
Then, learn a mapping function $f: X \rightarrow \{0, 1\}$ 