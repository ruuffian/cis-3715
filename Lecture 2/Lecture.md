January 19th, 2023

<h3> NumPy </h3>
Basic Array operations
```python
a = np.array([1,2,3])
b = np.array([4,5,6])

np.inner(a, b) # = [4, 10, 18]
```

<h3> SciKitLearn </h3>
Machine Learning library

![Sci Kit](images/scikit.png)

<h3> Other Tools </h3>
[PyTorch](https://pytorch.org) - Deep Learning tools developed by facebook
[TensorFlow](https://www.tensorflow.org) - Deep learning tools developed by google
[Matplotlib](https://matplotlib.org) - Plotting library in python

<h3> Python Basics </h3>
<center> <b>List</b> </center>

Ordered, Mutable, and allow duplicates. Lists are python's simplest array-like data set. It's syntax seems like an array in many other languages, but python doesn't support fixed-length arrays in this way.

```python
a = ["hello", "world", "bro"]
print(a[0]) # hello
print(a[-1]) # bro
print(a[0:2]) # ['hello', 'world']
print(a[0:-2]) # ['hello', 'world']
```
![List Example](images/lists.png)

There are three ways to add to a list- append, insert, and extend. They do exactly what they say, in classic python fashion.

Python lists can only have their elements removed by value, NOT by index-

```python
a = ["hi", "there"]
a.remove(0) # RUNTIME ERROR
a.remove("hi") # a = ["there"]
a = [0,2,0]
a.remove(0) # a = [2,0]
```

<center><b> Tuple </b></center>
Tuples are python's fixed-length array solution, hwoever they have an unfamiliar declaration syntax, seen below-

```python
a = ()
```