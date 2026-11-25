
# Problem 10 – Detecting Dependence

## Solution

Given:

\[
A = \begin{pmatrix}
1 & 2 & 3 \\
2 & 4 & 6 \\
0 & 1 & 5
\end{pmatrix}
\]

### 1. Identify the dependence between the rows

The second row is exactly twice the first row.

\[
R_2=2R_1
\]

Therefore, the rows of the matrix are linearly dependent.

### 2. Explain why the determinant is zero

A determinant is zero if the rows of a square matrix are linearly dependent.

Since the second row is a multiple of the first row:

\[
\boxed{\det(A)=0}
\]

This means the matrix does not have three linearly independent rows.

### 3. Connect the result with invertibility

A square matrix is invertible if and only if its determinant is nonzero.

In this case:

\[
\det(A)=0
\]

Therefore, the matrix is not invertible.

\[
\boxed{A^{-1}\text{ does not exist}}
\]

### Final Answer

The second row is twice the first row:

\[
R_2=2R_1
\]

Thus, the rows are linearly dependent, which means:

\[
\boxed{\det(A)=0}
\]

Since the determinant is zero, the matrix is not invertible.
