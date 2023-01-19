Step 1: Gather Data

![[example 1.png]]
- each row is an email

Step 2: Preprocess Data

![[preprocessing.png]]
- want to convert from english language to numerical values
- 'hello' and 'temple' exist in the email, so we add 1 to their dictionary values
- in this way we can represent each email numerically, allowing us to apply a ML algorithm
Example Emails as vectors:
```
[1 0 1 0 0]
[0 1 0 0 1]
[1 0 0 0 1]
```

Then, we take those vectors and input them into some ML model, for example a logistic regression model.

We want to build our classifier-
![[classifier.png]]

Then, from this classifier we have built we can actually evaluate our data.

![[evaluate.png]]

In this case, we can now use our model to determine whether an email is spam or not.
