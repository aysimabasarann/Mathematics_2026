
# Problem 04 – Triangular Matrix

## Solution

Given:

\[
A = \begin{pmatrix}
2 & 4 & 1 \\
0 & -3 & 5 \\
0 & 0 & 7
\end{pmatrix}
\]

### 1. Calculate the determinant

The matrix is an upper triangular matrix because all elements below the main diagonal are zero.

For a triangular matrix, the determinant is equal to the product of its diagonal entries.

Therefore:

\[
\det(A) = 2\cdot(-3)\cdot7
\]

\[
\det(A) = -6\cdot7
\]

\[
\boxed{\det(A)=-42}
\]

### 2. General rule for triangular matrices

The determinant of any upper or lower triangular matrix is the product of its main diagonal entries.

For an \(n\times n\) triangular matrix:

\[
\det(A)=a_{11}\cdot a_{22}\cdot\ldots\cdot a_{nn}
\]

### 3. Explanation

In this example, all entries below the main diagonal are zero.

Therefore, we do not need to expand the determinant or perform additional calculations.

We simply multiply the diagonal entries:

\[
2\cdot(-3)\cdot7=-42
\]

The same rule applies to lower triangular matrices.

### Final Answer

\[
\boxed{\det(A)=-42}
\]

The determinant of a triangular matrix is always the product of its main diagonal entries.
