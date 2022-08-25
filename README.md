# Quantum Computing

## Lesson 1: Linear Algebra for Quantum Computing

### Matrices

#### Types of matrices

- Column (one column matrix)
- Row (one row matrix)
- Square matrix (rows=columns)
- Equal matrices – two matrices considered equal if they have same dimensions & corresponding elements are equal
- Zero matrix – contains all 0s
- Identity matrix – multiplying a matrix by its identity matrix leaves it unchanged
  - to create an identity matrix just have all the elements along the main diagonal set to 1 and rest to 0
- Vector - either a single column or a single row
  - Vector length – computed with Pythagorean theorem (a^2 + b^2 = c^2)
    - $|| vector || = sqrt( x2 + y2 + … n^2 )$
    - Consider the vector [2, 3, 4]; x = 1, y = 3; so length: sqrt (4+9+16) = 5.38
    - A vector's nonnegative length is called the **norm** of the vector. Given vector v, this is written as ||v||
    - $|| v || = 1 \implies \text{v is a unit vector}$

#### Operations, Properties of Matrices

- Addition & subtraction – element-wise
- Matrix-Matrix Multiplication - multiply each row by each column
  - A x B -> number of columns in A must = # rows in B (inner dimensions must match); output dimensionality is # rows in A by # columns in B (i.e. outer dimensions of product matrices)
  - NOT COMMUTATIVE. Multiplication only commutative if A and B are both scalar values.
- Scalar-Matrix Multiplication - multiply each element in matrix by scalar
- Transposition – reverse order of rows & columns.
  - $(A^T)^T = A$ - transposing a transposition gives original matrix
  - $(cA)^T = cA^T$ - transposing the product of a scalar and a matrix A is the same as the multiplying the constant by the transposition of A
  - $(AB)^T = B^TA^T$ - Multiplying A by B and then transposing the product is equal to B transposed multiplied by A transposed
  - $(A+B)^T = A^T + B^T$ - transposing the sum of two equal-dimensioned matrices is the same as the sum of the individual transpositions
  - $S^T = S$ - if a **square** matrix is equal to its transpose, it's a **symmetric matrix**
- Submatrix – any portion of a matrix that remains after deleting any number of rows or coumns
- Determinant - the determinant of a matrix $A$ is denoted by $|A|$. Example in a generic form:
  - (2)(2) - (3)(1) = 1
  - Non-square matrices do not have determinants
  - The determinant of any square matrix A is a scalar, denoted $det(A)$
  - For 3x3 Matrices
    - Laplace Formula
    - Leibniz Formula
    - Sarrus' scheme
  - ![3x3 matrix det](img/determinant-3x3.png)
  - What are they for?
    - Finding eigenvalues and eigenvectors
    - Determining if the matrix has an inverse
    - Determining whether system of n equations in n unknowns has a solution
- Dot Product of two vectors (single column or single row)
  - $\sum_{i=1}^{n}X_iY_i$
  - ![dot product 3x1 by 3x1](img/dotprod.png)
  - if two vectors are both **orthogonal (perpendicular to each other)** and have unit length (length=1-> $||v_a||=1, ||v_b||=1$, the vectors are said to be **orthonormal**
  - The dot product is used to produce a single number (scalar) from two vertices or two matrices
  - Practical dot product uses, considering two vectors X and Y:
    - $cos \theta = (X \cdot Y) / ||X|| * ||Y||$
    - $ (X \cdot Y) = 0 \implies \text{vectors X and Y are perpendicular}$; this is because the cosine of a 90 degree angle is 0. The two vectors are referred to as **orthogonal**.
- Tensor Product
  - Tensor product of two vector spaces basically take the elements and multiplies them together. Here is a representation of a tensor product:
    - ![tensor product](img/tensorprod.png)
    - ![tensor product result](img/tensorprod2.png)

#### Vectors, Vector Spaces

- Spanning the Vector Space
  - A set of vectors $A_1, A_2, ... A_n$ is said to span a vector space $V$ if they are all in $V$ and every vector in $V$ can be expressed as a linear combination of the $A_1, A_2, ... A_n$ vectors.
  - Normally one will **omit the zero vector** as it does not really add anything to the definition
- Linear Dependence & Independence
  - A set of vectors $(V_1, V_2, ... V_n)$ are said to be **linearly dependent** if there is a set of $k_i$, not all zero, such that $k_1V_1 + k_2V_2 + ... + k_nV_n = 0$. If that is NOT the case, the vectors are **linearly independent**.
  - A **basis** for a **vector space** is a set of linearly independent vectors. Consider the following:
    - ![basis for vector space](img/basis.png)
- Orthonormal Basis
  - Basis: a **space** is totally defined by a set of vectors - **any point is a linear combination of the basis**.
  - Ortho-normal: orthogonal + normal
  - Orthogonal: dot product is 0
  - Normal: Magnitude is 1.
  - ![orthonormal basis](img/orthonormalbasis.png)
