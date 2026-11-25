
# Exercise 3 – When Does the Inverse Not Exist?

## Solution

Given:

\[
A=
\begin{pmatrix}
2&4\\
1&2
\end{pmatrix}
\]

### Method 1. Using the Determinant

For a 2×2 matrix:

\[
\det(A)=ad-bc
\]

\[
\det(A)=(2)(2)-(4)(1)
\]

\[
=4-4=0
\]

Since the determinant is zero, the matrix is not invertible.

Therefore:

\[
\boxed{A^{-1}\text{ does not exist.}}
\]

### Method 2. Using Dependence Between Rows

The rows of the matrix are:

\[
R_1=(2,4)
\]

\[
R_2=(1,2)
\]

Notice that:

\[
R_1=2R_2
\]

Therefore, the two rows are linearly dependent.

A matrix with linearly dependent rows cannot be invertible.

Thus:

\[
\boxed{A^{-1}\text{ does not exist.}}
\]

### Final Conclusion

Both methods give the same result:

- The determinant is zero.
- The rows are linearly dependent.

These two properties show that the matrix is not invertible.
