
# Problem 06 – Parameter and Invertibility

## Solution

Given:

\[
A(t)=\begin{pmatrix}
t & 1\\
2 & t
\end{pmatrix}
\]

### 1. Calculate the determinant

For a 2x2 matrix, the determinant is:

\[
\det(A)=ad-bc
\]

Substituting the values:

\[
\det(A(t))=t\cdot t-1\cdot2
\]

\[
\det(A(t))=t^2-2
\]

### 2. Find the values of t

A matrix is not invertible if and only if its determinant is zero.

Therefore:

\[
t^2-2=0
\]

\[
t^2=2
\]

Taking the square root:

\[
t=\pm\sqrt{2}
\]

Thus, the matrix is not invertible for:

\[
\boxed{t=\sqrt{2}\text{ or }t=-\sqrt{2}}
\]

### 3. Explanation

When the determinant of a square matrix is zero, the matrix has no inverse.

For all other values of t, the determinant is nonzero, so the matrix is invertible.

### Final Answer

\[
\boxed{t\in\{-\sqrt{2},\sqrt{2}\}}
\]

The matrix is not invertible exactly when its determinant equals zero.
