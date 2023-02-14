February 14th, 2023

Summary of What I think I missed:
- Build Model
	- $f(x_i) = w_0 + w_1x_{i,1} + w_2x_{i,2} \dots w_dx_{i, d}$ 
- Split the data set, about 70/30 training and testing.
- Gradient Descent
	- $x_{t+1} = x_t - n \nabla f(x_t)$ 
	- Basically move in the opposite direction of the gradient to minimize the loss function ($f(x_t)$).
	- Example: Linear Regression - $min_w ||y - Xw||^2$ has gradient $-2X^T(y-Xw)$, so gradient descent looks like this:
		- $w_{t+1} = w_t - n(2X^T(Xw_t - y))$
- Overfitting: Errors on training data is very good, but errors on new data points are very large.
	- How to avoid? add a regularization term