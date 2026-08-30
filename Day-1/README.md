# NumPy Assignment 1 – Array Indexing & Slicing

## Overview

This assignment covers NumPy array creation, indexing, slicing, row extraction, column extraction, and advanced slicing using both **2D and 3D arrays**.

---

# Part 1 – 3D Array Indexing & Slicing

## Create 3D Array

```python
import numpy as np

arr = np.array([
    [
        [10, 11, 12, 13, 14],
        [15, 16, 17, 18, 19],
        [20, 21, 22, 23, 24],
        [25, 26, 27, 28, 29]
    ],
    [
        [30, 31, 32, 33, 34],
        [35, 36, 37, 38, 39],
        [40, 41, 42, 43, 44],
        [45, 46, 47, 48, 49]
    ],
    [
        [50, 51, 52, 53, 54],
        [55, 56, 57, 58, 59],
        [60, 61, 62, 63, 64],
        [65, 66, 67, 68, 69]
    ]
])

print(arr.shape)
```

Output:

```text
(3, 4, 5)
```

- 3 matrices
- 4 rows in each matrix
- 5 columns in each row

---

# Section A – Access Individual Elements

### Extract:

- 10
- 24
- 37
- 43
- 54
- 66
- 58
- 49

```python
print(arr[0, 0, 0])  # 10
print(arr[0, 2, 4])  # 24
print(arr[1, 1, 2])  # 37
print(arr[1, 2, 3])  # 43
print(arr[2, 0, 4])  # 54
print(arr[2, 3, 1])  # 66
print(arr[2, 1, 3])  # 58
print(arr[1, 3, 4])  # 49
```

---

# Section B – Access Complete Rows

### 1. `[15, 16, 17, 18, 19]`

```python
print(arr[0, 1, :])
```

### 2. `[40, 41, 42, 43, 44]`

```python
print(arr[1, 2, :])
```

### 3. `[65, 66, 67, 68, 69]`

```python
print(arr[2, 3, :])
```

---

# Section C – Access Complete 2D Matrices

### First Matrix

```python
print(arr[0])
```

### Second Matrix

```python
print(arr[1])
```

### Third Matrix

```python
print(arr[2])
```

---

# Section D – Column Extraction

### 1. `[10, 15, 20, 25]`

```python
print(arr[0, :, 0])
```

### 2. `[32, 37, 42, 47]`

```python
print(arr[1, :, 2])
```

### 3. `[54, 59, 64, 69]`

```python
print(arr[2, :, 4])
```

---

# Section E – Slicing

## 1. First Two Matrices

```python
print(arr[:2])
```

## 2. Last Two Matrices

```python
print(arr[1:])
```

## 3. First Two Rows From Every Matrix

```python
print(arr[:, :2, :])
```

## 4. Last Two Rows From Every Matrix

```python
print(arr[:, 2:, :])
```

## 5. First Three Columns From Every Matrix

```python
print(arr[:, :, :3])
```

## 6. Last Two Columns From Every Matrix

```python
print(arr[:, :, 3:])
```

---

# Section F – Advanced Slicing

## 1. Extract

```text
[
 [10, 11, 12],
 [15, 16, 17]
]
```

```python
print(arr[0, :2, :3])
```

## 2. Extract

```text
[
 [42, 43, 44],
 [47, 48, 49]
]
```

```python
print(arr[1, 2:, 2:])
```

## 3. Extract

```text
[
 [55, 56],
 [60, 61],
 [65, 66]
]
```

```python
print(arr[2, 1:, :2])
```

## 4. Extract

```text
[
 [13, 14],
 [18, 19]
]
```

```python
print(arr[0, :2, 3:])
```

---

# Section G – Advanced Questions

## 1. Every Alternate Matrix

```python
print(arr[::2])
```

## 2. Every Alternate Row From All Matrices

```python
print(arr[:, ::2, :])
```

## 3. Every Alternate Column From All Matrices

```python
print(arr[:, :, ::2])
```

## 4. First Column From Every Matrix

```python
print(arr[:, :, 0])
```

## 5. Last Column From Every Matrix

```python
print(arr[:, :, -1])
```

## 6. Middle Row From Every Matrix

```python
print(arr[:, 2, :])
```

## 7. Middle Column From Every Matrix

```python
print(arr[:, :, 2])
```

## 8. Reverse the Order of Matrices

```python
print(arr[::-1])
```

## 9. Reverse the Rows Inside Every Matrix

```python
print(arr[:, ::-1, :])
```

## 10. Reverse the Columns Inside Every Matrix

```python
print(arr[:, :, ::-1])
```

---

# Part 2 – 2D Array Indexing & Slicing

## Create 2D Array

```python
import numpy as np

arr = np.array([
    [10, 11, 12, 13, 14, 15],
    [20, 21, 22, 23, 24, 25],
    [30, 31, 32, 33, 34, 35],
    [40, 41, 42, 43, 44, 45],
    [50, 51, 52, 53, 54, 55],
    [60, 61, 62, 63, 64, 65]
])

print(arr.shape)
```

Output:

```text
(6, 6)
```

---

# 1. Every Alternate Row

### Expected Output

```text
[
 [10, 11, 12, 13, 14, 15],
 [30, 31, 32, 33, 34, 35],
 [50, 51, 52, 53, 54, 55]
]
```

```python
print(arr[::2])
```

---

# 2. Every Alternate Column

### Expected Output

```text
[
 [10, 12, 14],
 [20, 22, 24],
 [30, 32, 34],
 [40, 42, 44],
 [50, 52, 54],
 [60, 62, 64]
]
```

```python
print(arr[:, ::2])
```

---

# 3. First Column

### Expected Output

```text
[10, 20, 30, 40, 50, 60]
```

```python
print(arr[:, 0])
```

---

# 4. Last Column

### Expected Output

```text
[15, 25, 35, 45, 55, 65]
```

```python
print(arr[:, -1])
```

---

# 5. Middle Row

### Expected Output

```text
[40, 41, 42, 43, 44, 45]
```

```python
print(arr[3, :])
```

---

# 6. Middle Column

### Expected Output

```text
[13, 23, 33, 43, 53, 63]
```

```python
print(arr[:, 3])
```

---

# 7. First Three Rows

### Expected Output

```text
[
 [10, 11, 12, 13, 14, 15],
 [20, 21, 22, 23, 24, 25],
 [30, 31, 32, 33, 34, 35]
]
```

```python
print(arr[:3])
```

---

# 8. Last Three Rows

### Expected Output

```text
[
 [40, 41, 42, 43, 44, 45],
 [50, 51, 52, 53, 54, 55],
 [60, 61, 62, 63, 64, 65]
]
```

```python
print(arr[3:])
```

---

# 9. First Three Columns

### Expected Output

```text
[
 [10, 11, 12],
 [20, 21, 22],
 [30, 31, 32],
 [40, 41, 42],
 [50, 51, 52],
 [60, 61, 62]
]
```

```python
print(arr[:, :3])
```

---

# 10. Last Three Columns

### Expected Output

```text
[
 [13, 14, 15],
 [23, 24, 25],
 [33, 34, 35],
 [43, 44, 45],
 [53, 54, 55],
 [63, 64, 65]
]
```

```python
print(arr[:, 3:])
```

---

# 11. Reverse All Rows

### Expected Output

```text
[
 [60, 61, 62, 63, 64, 65],
 [50, 51, 52, 53, 54, 55],
 [40, 41, 42, 43, 44, 45],
 [30, 31, 32, 33, 34, 35],
 [20, 21, 22, 23, 24, 25],
 [10, 11, 12, 13, 14, 15]
]
```

```python
print(arr[::-1])
```

---

# 12. Reverse All Columns

### Expected Output

```text
[
 [15, 14, 13, 12, 11, 10],
 [25, 24, 23, 22, 21, 20],
 [35, 34, 33, 32, 31, 30],
 [45, 44, 43, 42, 41, 40],
 [55, 54, 53, 52, 51, 50],
 [65, 64, 63, 62, 61, 60]
]
```

```python
print(arr[:, ::-1])
```

---

# 13. Reverse Rows and Columns Simultaneously

### Expected Output

```text
[
 [65, 64, 63, 62, 61, 60],
 [55, 54, 53, 52, 51, 50],
 [45, 44, 43, 42, 41, 40],
 [35, 34, 33, 32, 31, 30],
 [25, 24, 23, 22, 21, 20],
 [15, 14, 13, 12, 11, 10]
]
```

```python
print(arr[::-1, ::-1])
```

---

# Additional Advanced Slicing Questions

## 1. Extract

```text
[
 [22, 23, 24],
 [32, 33, 34],
 [42, 43, 44]
]
```

```python
print(arr[1:4, 2:5])
```

---

## 2. Extract

```text
[
 [11, 13, 15],
 [31, 33, 35],
 [51, 53, 55]
]
```

```python
print(arr[::2, 1::2])
```

---

## 3. Extract

```text
[
 [40, 41, 42, 43, 44, 45],
 [50, 51, 52, 53, 54, 55]
]
```

```python
print(arr[3:5, :])
```

---

## 4. Extract

```text
[
 [14, 15],
 [24, 25],
 [34, 35],
 [44, 45],
 [54, 55],
 [64, 65]
]
```

```python
print(arr[:, 4:6])
```

---

# NumPy Indexing & Slicing Syntax

## Basic Indexing

```python
arr[row, column]
```

## General Slicing

```python
arr[start:stop:step]
```

## 2D Slicing

```python
arr[row_start:row_stop:row_step,
    column_start:column_stop:column_step]
```

## 3D Slicing

```python
arr[matrix_start:matrix_stop:matrix_step,
    row_start:row_stop:row_step,
    column_start:column_stop:column_step]
```

---

# Common Examples

```python
arr[:3]          # First 3 rows
arr[3:]          # Last 3 rows

arr[:, :3]       # First 3 columns
arr[:, 3:]       # Last 3 columns

arr[::2]         # Every alternate row
arr[:, ::2]      # Every alternate column

arr[::-1]        # Reverse rows
arr[:, ::-1]     # Reverse columns

arr[::-1, ::-1]  # Reverse rows and columns
```

---

# Key Concepts Learned

- Creating NumPy arrays
- Understanding array dimensions
- Understanding `shape`
- Zero-based indexing
- Accessing individual elements
- Accessing complete rows
- Accessing complete columns
- Accessing complete matrices
- Basic slicing
- Advanced slicing
- Alternate row selection
- Alternate column selection
- Negative indexing
- Reversing arrays
- Combining row and column slicing
- 2D array indexing
- 3D array indexing

---

# Conclusion

This assignment provides practical experience with **NumPy indexing and slicing** for both 2D and 3D arrays.

These concepts are fundamental for:

- Data Science
- Data Analysis
- Machine Learning
- Artificial Intelligence
- Python Programming
