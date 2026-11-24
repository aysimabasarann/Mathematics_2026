
# Problem 07 – Using Properties Instead of Recomputing

## Solution

Given:

\[
\det(A)=-4
\]

where A is a 3x3 matrix.

### 1. Calculate det(2A)

For an n x n matrix, the determinant property is:

\[
\det(kA)=k^n\det(A)
\]

Since A is a 3x3 matrix:

\[
\det(2A)=2^3\det(A)
\]

Substituting:

\[
\det(2A)=8\cdot(-4)
\]

\[
\boxed{\det(2A)=-32}
\]

### 2. Calculate det(A^T)

The determinant of a matrix is equal to the determinant of its transpose.

Therefore:

\[
\det(A^T)=\det(A)
\]

\[
\boxed{\det(A^T)=-4}
\]

### 3. Calculate det(A^2)

Using the determinant property:

\[
\det(AB)=\det(A)\det(B)
\]

We obtain:

\[
\det(A^2)=\det(A)\cdot\det(A)
\]

\[
\det(A^2)=(-4)(-4)
\]

\[
\boxed{\det(A^2)=16}
\]

### 4. Calculate det(-A)

For a 3x3 matrix:

\[
\det(-A)=(-1)^3\det(A)
\]

Substituting:

\[
\det(-A)=-1\cdot(-4)
\]

\[
\boxed{\det(-A)=4}
\]

### Final Answer

\[
\boxed{\det(2A)=-32}
\]

\[
\boxed{\det(A^T)=-4}
\]

\[
\boxed{\det(A^2)=16}
\]

\[
\boxed{\det(-A)=4}
\]

All results were obtained using determinant properties instead of recalculating the determinants from the matrix entries.
