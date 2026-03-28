# 🔢 NumPy - Full Course Notebook

> A complete, beginner-to-advanced NumPy learning resource built as an interactive Jupyter Notebook - with a real-world capstone project.

[![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://python.org)
[![NumPy](https://img.shields.io/badge/NumPy-1.24+-013243?style=for-the-badge&logo=numpy&logoColor=white)](https://numpy.org)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?style=for-the-badge&logo=jupyter&logoColor=white)](https://jupyter.org)
[![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)](LICENSE)

---

## 🗂️ Repository Contents

### `NumPy_Full_Course.ipynb`

| Section | Topic | Key Concepts |
|---------|-------|-------------|
| 1 | 📌 Introduction | Why NumPy, speed & memory comparison |
| 2 | ⚡ Creating Array| creating structured arrays |
| 3 | 🧱 Basics | ndarray, dtypes, factory functions, attributes |
| 4 | 🔍 Indexing & Slicing | Basic, fancy, boolean — view vs copy |
| 5 | 🔄 Reshaping | reshape, ravel, flatten, stack, split |
| 6 | ✏️ Modification | append, insert, clip, sort, argsort, pad |
| 7 | 📡 Broadcasting | Rules, normalisation, vectorisation speed |
| 8 | ❓ Missing Values | NaN, nan-safe functions, imputation |
| 9 | 📊 Statistics | Aggregation, percentiles, correlation, histogram |
| 10 | 🔗 Linear Algebra | matmul, solve, eig, SVD, lstsq, norms |
|   | 🏆 Capstone Project| 50-student analytics pipeline |

---

## 🚀 Getting Started

### Prerequisites

```
Python 3.10 or higher
NumPy 1.24 or higher
Jupyter Notebook or JupyterLab
```

### Installation

```bash
# 1. Clone the repository
git clone https://github.com/Purvijain1234/Python-by-Purvi-Jain.git
cd Python-by-Purvi-Jain/NumPy

# 2. Install dependencies
pip install numpy jupyter

# 3. Launch Jupyter
jupyter notebook
```

### Open in VS Code

1. Install the **Jupyter** extension
2. Open any `.ipynb` file
3. Click **Run All** or run cells one by one

---

## 💡 Key Concepts at a Glance

### Why NumPy?

```python
import numpy as np

# Python list — slow
result = [x * 2 for x in range(1_000_000)]   # ~0.08s

# NumPy array — fast
arr    = np.arange(1_000_000)
result = arr * 2                              # ~0.001s  → 80× faster
```

### Creating Arrays

```python
np.array([1, 2, 3])          # from list
np.zeros((3, 4))             # all zeros
np.ones((2, 3))              # all ones
np.arange(0, 10, 2)         # [0, 2, 4, 6, 8]
np.linspace(0, 1, 5)        # [0, 0.25, 0.5, 0.75, 1.0]
np.random.default_rng(42).random((3, 3))  # random
```

### Indexing & Slicing

```python
arr[2]          # single element
arr[1:5]        # slice (VIEW)
arr[[0, 2, 4]]  # fancy index (COPY)
arr[arr > 5]    # boolean mask (COPY)
arr[1:4].copy() # force a copy
```

### Broadcasting

```python
# Operations on different-shaped arrays
a = np.array([[1, 2, 3],
              [4, 5, 6]])       # shape (2, 3)
b = np.array([10, 20, 30])     # shape    (3,)
a + b                           # → shape (2, 3) ✅
```

### Handling Missing Values

```python
data = np.array([1.0, np.nan, 3.0, np.nan, 5.0])

np.isnan(data)          # [F, T, F, T, F]
np.nanmean(data)        # 3.0  — ignores NaN
np.nansum(data)         # 9.0  — ignores NaN

# Impute with mean
data[np.isnan(data)] = np.nanmean(data)
```

### Linear Algebra

```python
A = np.array([[2, 1], [5, 3]])
b = np.array([5, 13])

A @ b                       # matrix × vector
np.linalg.solve(A, b)      # solve Ax = b → [2, 1]
np.linalg.inv(A)           # matrix inverse
np.linalg.det(A)           # determinant
```

---

## 📊 Capstone Project Preview

The easy capstone (`NumPy_Capstone_Project.ipynb`) analyses data for **50 students** across **4 subjects**:

```
=========================================================
        STUDENT EXAM — FINAL REPORT CARD
=========================================================

  CLASS OVERVIEW
  ----------------------------------------
  Total students     : 50
  Subjects           : Maths, Science, English, CompSci
  Class average      : 67.83
  Highest score      : 91.40  (Pooja)
  Lowest score       : 39.20  (Farhan)
  Pass rate (>=40)   : 48/50 = 96%

  GRADE SUMMARY
  ----------------------------------------
  Grade A : 12 students (24%)
  Grade B : 18 students (36%)
  Grade C : 12 students (24%)
  Grade D :  6 students (12%)
  Grade F :  2 students  (4%)

  SUBJECT RANKING (best → worst)
  ----------------------------------------
  1. English     : 70.54
  2. CompSci     : 69.22
  3. Science     : 66.87
  4. Maths       : 64.71

  STUDY HOURS INSIGHT
  ----------------------------------------
  Correlation (hours vs score): r = 0.731
  Each extra hour adds ~2.4 marks

  ✅ Analysis complete using only NumPy!
```

---

## 🗃️ File Structure

```
NumPy/
├── 1- Numpy Introduction.ipynb
├── 2 - Creating Array.ipynb
├── 3 - Numpy Basics.ipynb
├── 4 - Indexing & Slicing.ipynb
├── 5 - Reshaping & Manipulation.ipynb
├── 6 - Array Modification.ipynb
├── 7 - Broadcasting & Vectorisation.ipynb
├── 8 - Handling Missing Values.ipynb
├── 9 - Math & Stats.ipynb
├── 10 - Linear Algebra.ipynb
└── README.md 
```

---

## 👩‍💻 Author

**Purvi Jain**

[![GitHub](https://img.shields.io/badge/GitHub-Purvijain1234-181717?style=flat-square&logo=github)](https://github.com/Purvijain1234)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Purvi_Jain-0A66C2?style=flat-square&logo=linkedin)](https://linkedin.com/in/purvi-jain-315683326)

---

<div align="center">

⭐ **If this helped you, please star the repo!** ⭐

*Part of the [Python by Purvi Jain](https://github.com/Purvijain1234/Python-by-Purvi-Jain) learning series*

</div>
