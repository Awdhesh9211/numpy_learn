# 🧠 NumPy Revision Guide (With Output + Short Explanations)

---

# 📌 1. What is NumPy?

NumPy is a Python library for fast numerical computation using arrays.

👉 Core object: `ndarray`
👉 Think: List ➝ upgraded into math engine ⚡

---

# 🏁 2. Origin & Problem Solved

* Created by Travis Oliphant (2005)
* Problem:

  * Python lists are slow
  * No matrix support
  * High memory usage

✅ Solution:

* Fast (C backend)
* Vectorized (no loops)
* Built-in linear algebra

---

# 📦 3. Array Creation

```python
import numpy as np

a = np.array([1,2,3])
print(a)
```

Output:

```
[1 2 3]
```

👉 Creates array

---

# 🔍 4. Properties

```python
print(a.shape)
print(a.ndim)
```

Output:

```
(3,)
1
```

👉 Shape = size, ndim = dimensions

---

# ✂️ 5. Indexing

```python
print(a[1])
```

Output:

```
2
```

👉 Access element

---

# 🔄 6. Reshape

```python
a = np.arange(6)
print(a.reshape(2,3))
```

Output:

```
[[0 1 2]
 [3 4 5]]
```

👉 Change shape

---

# ➕ 7. Operations

```python
a = np.array([1,2,3])
b = np.array([4,5,6])
print(a + b)
```

Output:

```
[5 7 9]
```

👉 Element-wise addition

---

# 📊 8. Math Functions

```python
print(np.mean(a))
```

Output:

```
2.0
```

👉 Average

---

# 🔢 9. Broadcasting

```python
print(a + 2)
```

Output:

```
[3 4 5]
```

👉 Adds scalar to all elements

---

# 🔍 10. Filtering

```python
print(a[a > 1])
```

Output:

```
[2 3]
```

👉 Condition-based selection

---

# 🧱 11. CRUD Operations

## CREATE

```python
a = np.array([1,2,3])
a = np.append(a, 4)
print(a)
```

Output:

```
[1 2 3 4]
```

👉 Add element

## READ

```python
print(a[2])
```

Output:

```
3
```

👉 Access value

## UPDATE

```python
a[1] = 10
print(a)
```

Output:

```
[ 1 10  3  4]
```

👉 Modify value

## DELETE

```python
a = np.delete(a, 0)
print(a)
```

Output:

```
[10  3  4]
```

👉 Remove element

---

# 🧮 12. Matrix Operations

```python
A = np.array([[1,2],[3,4]])
B = np.array([[5,6],[7,8]])

print(A + B)
```

Output:

```
[[ 6  8]
 [10 12]]
```

👉 Matrix addition

```python
print(A @ B)
```

Output:

```
[[19 22]
 [43 50]]
```

👉 Matrix multiplication

```python
print(A.T)
```

Output:

```
[[1 3]
 [2 4]]
```

👉 Transpose

```python
print(np.linalg.det(A))
```

Output:

```
-2.0
```

👉 Determinant

```python
print(np.linalg.inv(A))
```

Output:

```
[[-2.   1. ]
 [ 1.5 -0.5]]
```

👉 Inverse

---

# 🎲 13. Random

```python
np.random.seed(1)
print(np.random.randint(1,5))
```

Output:

```
2
```

👉 Random number

---

# 📁 14. Save & Load

```python
np.save('a.npy', a)
b = np.load('a.npy')
print(b)
```

Output:

```
[10  3  4]
```

👉 Store & retrieve data

---

# 🧠 15. Key Concepts

* ndarray is fast
* No loops needed
* Fixed size arrays

---

# ⚡ 16. When NOT to Use

* Frequent insert/delete → use list
* Table data → use pandas

---

# 🎯 Final Summary

NumPy = speed + math + efficiency ⚡

👉 Backbone of Data Science & ML

---

💡 Revise → Practice → Master 🚀
