# Assignments README

This repository contains two assignments covering **Python/NumPy
fundamentals** and **Linear Algebra fundamentals for Artificial
Intelligence**.

------------------------------------------------------------------------

# Assignment 1 --- Python: 3D Arrays & Dictionaries

## Overview

This assignment focuses on Python programming using **NumPy 3D arrays**
and **dictionaries**.

## Part A --- 3D Arrays

### Q1 --- Create and Access a 3D Array

Create the given 3D array and: - Print the complete 3D array. - Print
the first layer. - Print the second row of the second layer. - Print
element `11`.

### Q2 --- Reverse the Order of Layers

Reverse the layers of the 3D array.

``` python
arr[::-1]
```

### Q3 --- Reverse Every Row

Reverse the elements of every row inside every layer.

``` python
arr[:, :, ::-1]
```

### Q4 --- Completely Reverse the 3D Array

Reverse: 1. The order of layers. 2. The order of rows inside each layer.
3. The elements inside every row.

``` python
arr[::-1, ::-1, ::-1]
```

------------------------------------------------------------------------

## Part B --- Dictionaries

### Q5 --- Student Dictionary

Create a dictionary containing: - Roll No - Name - Age - Department -
CGPA

Display all information.

### Q6 --- Update Dictionary

Using the student dictionary: - Update CGPA to `9.2`. - Add `City` with
value `Chennai`. - Display the updated dictionary.

### Q7 --- Dictionary Methods

Use appropriate dictionary methods to display: - All keys --- `keys()` -
All values --- `values()` - All key-value pairs --- `items()`

### Q8 --- Nested Dictionary

Create a nested dictionary containing three students with their: -
Name - Age

Practice: - Accessing nested values. - Printing specific student
information. - Displaying all student names using a loop.

### Q9 --- Product Dictionary

Create a dictionary containing five products.

Each product contains: - Product Name - Price - Quantity

Tasks: - Display all products. - Find the product with the highest
price. - Calculate total inventory value.

**Formula:**

``` text
Inventory Value = Price × Quantity
```

### Q10 --- Student Marks Dictionary

Create a dictionary containing five students and their marks.

Tasks: - Find the student with the highest marks. - Find the student
with the lowest marks. - Calculate average marks. - Display students who
scored more than `85`.

------------------------------------------------------------------------

# Assignment 2 --- Fundamentals of Linear Algebra for Artificial Intelligence

## Overview

This assignment covers fundamental linear algebra concepts used in
Artificial Intelligence.

## Part A --- Scalars, Vectors and Matrices

### Q1

Identify: - Scalar - Vector - Matrix - Tensor

### Q2

Determine matrix dimensions.

### Q3

Perform: - Matrix addition - Matrix subtraction - Scalar multiplication

### Q4

Find the transpose of a matrix.

### Q5

Find the transpose of another matrix.

------------------------------------------------------------------------

## Part B --- Matrix Multiplication

### Q6

Multiply two matrices.

### Q7

Determine whether matrix multiplications are possible and identify the
resulting dimensions.

**Rule:**

``` text
(m × n)(n × p) = (m × p)
```

The inner dimensions must match.

### Q8

Calculate matrix multiplication `AB`.

### Q9

Verify whether matrix multiplication is commutative by calculating:

``` text
AB
BA
```

Conclusion:

``` text
AB ≠ BA
```

in general, so matrix multiplication is **not commutative**.

------------------------------------------------------------------------

## Part C --- Vector Operations

### Q10

Find the magnitude of a vector.

**Formula:**

``` text
|x| = √(x₁² + x₂² + ... + xₙ²)
```

### Q11

Find the magnitude of a three-dimensional vector.

### Q12

Calculate the dot product of two vectors.

**Formula:**

``` text
x · y = x₁y₁ + x₂y₂ + ... + xₙyₙ
```

### Q13

Determine whether two vectors are orthogonal.

Two vectors are orthogonal when:

``` text
x · y = 0
```

### Q14

Normalize a vector.

**Formula:**

``` text
x̂ = x / |x|
```

### Q15

Calculate Euclidean distance between two points.

**Formula:**

``` text
d(A,B) = √((x₂-x₁)² + (y₂-y₁)²)
```

------------------------------------------------------------------------

## Part D --- Vector Spaces and Span

### Q16 --- Linear Independence

Determine whether vectors are linearly independent or dependent.

If one vector is a scalar multiple of another, the vectors are
**linearly dependent**.

### Q17 --- Span

Determine whether a vector belongs to the span of two given vectors by
solving for their linear combination.

### Q18 --- Basis

Find a basis for `R²`.

A standard basis is:

``` text
{ [1, 0], [0, 1] }
```

### Q19 --- Rank

Find the rank of a matrix with dependent rows.

### Q20 --- Rank

Find the rank of a matrix with independent rows.

------------------------------------------------------------------------

## Part E --- Orthogonality

### Q21

Determine whether given pairs of vectors are orthogonal using their dot
products.

### Q22 --- Cosine Similarity

Calculate cosine similarity using:

``` text
cos(θ) = (x · y) / (|x| |y|)
```

Interpretation:

``` text
Close to 1  → Similar direction
Close to 0  → Nearly perpendicular
Close to -1 → Opposite direction
```

For the assignment example, the cosine similarity is approximately
**0.98**, meaning the vectors point in very similar directions.

### Q23 --- Key Concepts

Explain the difference between:

#### Orthogonal Vectors

Vectors whose dot product is zero.

#### Orthonormal Vectors

Vectors that are orthogonal to each other and each have magnitude one.

#### Basis

A set of linearly independent vectors that spans a vector space.

#### Vector Space

A collection of vectors that supports vector addition and scalar
multiplication according to vector-space rules.

------------------------------------------------------------------------

# Learning Path

``` text
Assignment 1
    ↓
Python
    ↓
NumPy
    ↓
3D Arrays
    ↓
Indexing & Slicing
    ↓
Dictionaries
    ↓
Nested Dictionaries
    ↓
Loops & Calculations

Assignment 2
    ↓
Scalars / Vectors / Matrices / Tensors
    ↓
Matrix Operations
    ↓
Matrix Multiplication
    ↓
Vector Operations
    ↓
Dot Product / Magnitude
    ↓
Orthogonality / Normalization
    ↓
Span / Basis
    ↓
Rank
    ↓
Cosine Similarity
    ↓
Vector Spaces
```

## Summary

  Assignment     Main Focus
  -------------- -------------------------------------------------------
  Assignment 1   Python, NumPy 3D arrays, slicing, dictionaries, loops
  Assignment 2   Linear Algebra fundamentals for AI

Together, these assignments provide a foundation in **Python programming
and the mathematical concepts used in Artificial Intelligence**.
