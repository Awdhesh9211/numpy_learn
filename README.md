# 🧠 NumPy Revision Guide (One-Stop Cheat Sheet)

---

# 📌 1. What is NumPy?

**NumPy (Numerical Python)** is a Python library used for fast numerical computations using multi-dimensional arrays.

👉 Core object: `ndarray`

---

# 🏁 2. Origin & Why NumPy Exists

### 📜 Origin

* Created by **Travis Oliphant (2005)**
* Built on older libraries: Numeric + Numarray

### ❗ Problems it Solves

* Python lists are slow for numerical operations
* No built-in support for matrix/linear algebra
* Memory inefficient

### ✅ NumPy Solves:

* Fast computation (C backend)
* Vectorized operations (no loops)
* Efficient memory usage
* Built-in linear algebra support

---

# ⚙️ 3. Installation

```bash
pip install numpy
```

```python
import numpy as np
```

---

# 📦 4. Array Creation

```python
np.array([1,2,3])
np.zeros((2,3))
np.ones((2,2))
np.eye(3)
np.arange(0,10,2)
np.linspace(0,1,5)
```

---

# 🔍 5. Array Properties

```python
a.shape
a.ndim
a.size
a.dtype
```

---

# ✂️ 6. Indexing & Slicing

```python
a[0]
a[1:3]

b[0,1]
b[:,1]
b[0,:]
```

---

# 🔄 7. Reshaping

```python
a.reshape(2,3)
```

---

# ➕ 8. Operations (Vectorization)

```python
a + b
a - b
a * b
a ** 2
```

---

# 📊 9. Math Functions

```python
np.sum(a)
np.mean(a)
np.min(a)
np.max(a)
np.std(a)
```

---

# 🔢 10. Broadcasting

```python
a + 2
```

---

# 🔍 11. Filtering

```python
a[a > 3]
```

---

# 🔁 12. Iteration

```python
for x in a:
    print(x)
```

---

# 🧱 13. CRUD Operations

## ✅ CREATE

```python
np.append(arr, 4)
np.insert(arr, 1, 10)
```

## 👀 READ

```python
arr[0]
arr[arr > 5]
```

## ✏️ UPDATE

```python
arr[1] = 100
arr[arr > 50] = 0
```

## ❌ DELETE

```python
np.delete(arr, 1)
```

⚠️ Note: NumPy arrays are fixed size → operations create new arrays

---

# 🧮 14. Matrix Operations

```python
A + B
A - B
A * B            # element-wise
A @ B            # matrix multiplication
A.T              # transpose
np.linalg.inv(A)
np.linalg.det(A)
np.trace(A)
np.linalg.matrix_power(A, 2)
np.linalg.eig(A)
np.linalg.solve(A, b)
```

---

# 🎲 15. Random

```python
np.random.rand(2,2)
np.random.randint(1,10)
np.random.seed(42)
```

---

# 📁 16. Save & Load

```python
np.save('file.npy', a)
np.load('file.npy')
```

---

# 🧠 17. Key Concepts to Remember

* `ndarray` is faster than list
* Vectorization > loops
* Broadcasting simplifies operations
* NumPy = foundation of Data Science & ML

---

# ⚡ 18. When NOT to Use NumPy

* Frequent insert/delete → use list
* Tabular data → use Pandas

---

# 🚀 19. Quick Practice

```python
arr = np.arange(1,11)

print(arr[arr % 2 == 0])
print(arr.reshape(2,5))
print(np.mean(arr))
```

---

# 🎯 Final Summary

NumPy is:

* Fast ⚡
* Memory efficient 🧠
* Math-focused 🔢

👉 It turns Python into a scientific computing powerhouse.

---

# 🔥 Next Steps

* Learn Pandas (data handling)
* Learn Matplotlib (visualization)
* Learn Machine Learning

---

💡 Tip: Revise this once → Practice twice → You’ll remember forever.
