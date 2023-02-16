February 16th, 2023

First, we go over quiz answers- I got all 3 T/F and the question on hwo to avoid overfitting. The objective function for linear regression I got hilariously wrong. This is the objective function of linear regression: $min_w \thinspace ||Y - Xw||_2$

*Negative log-likelihood function*: $\sum_{j=1}^n \left \{y_iw^Tx_i - log(1 + exp(w^Tx_i)) \right\}$ 

Use gradient descent to optimize the loss function.

Loss Function: $min_w \thinspace \sum_{i=1}^n log(1 + exp(w^Tx_i)) - y_iw^Tx_i$
Gradient of Loss Function: $\frac{\delta L}{\delta w} = \sum_{i=1}^n x_i \left( y_i - \frac{w^Tx_i}{1+exp)w^Tx_i} \right)$

### Linear vs Logistic Regression

| Type     | Features           |
| -------- | ------------------ |
| Linear   | - Y is continuous, |
| Logistic | - Y is discrete                   |

**Linear**: $f(x_i) = w_0 +w_1x_1 \dots w_dx_d$
Logistic: $f(x_i) = \frac{1}{1+exp(w^Tx_i)}$

![[regression.png]]

How do we evaluate our classification alg?

For logistic regression, when the data is balanced (roughly same amount of 0s and 1s), we simply take how many correct predictions we made and divide it by the total number of predictions.
![[evaluation.png]]