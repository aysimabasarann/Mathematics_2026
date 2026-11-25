
# Exercise 6 – Solving a System Using the Inverse

## Solution

Given:

\[
Ax=b
\]

where

\[
A=
\begin{pmatrix}
2&1\\
1&3
\end{pmatrix},
\qquad
b=
\begin{pmatrix}
5\\
7
\end{pmatrix}
\]

### Step 1. Find the Inverse of A

For a 2×2 matrix:

\[
A^{-1}=\frac{1}{ad-bc}
\begin{pmatrix}
d&-b\\
-c&a
\end{pmatrix}
\]

First, calculate the determinant:

\[
\det(A)=(2)(3)-(1)(1)
\]

\[
=6-1=5
\]

Therefore:

\[
A^{-1}=
\frac{1}{5}
\begin{pmatrix}
3&-1\\
-1&2
\end{pmatrix}
\]

### Step 2. Calculate x Using x = A⁻¹b

\[
x=A^{-1}b
\]

Substitute the values:

\[
x=
\frac{1}{5}
\begin{pmatrix}
3&-1\\
-1&2
\end{pmatrix}
\begin{pmatrix}
5\\
7
\end{pmatrix}
\]

Multiply the matrices:

\[
x=
\frac{1}{5}
\begin{pmatrix}
15-7\\
-5+14
\end{pmatrix}
\]

\[
x=
\frac{1}{5}
\begin{pmatrix}
8\\
9
\end{pmatrix}
\]

Therefore:

\[
\boxed{
x=
\begin{pmatrix}
\frac85\\
\frac95
\end{pmatrix}
}
\]

### Step 3. Verify the Result

Substitute the solution back into the original equation:

\[
Ax=
\begin{pmatrix}
2&1\\
1&3
\end{pmatrix}
\begin{pmatrix}
\frac85\\
\frac95
\end{pmatrix}
\]

\[
=
\begin{pmatrix}
\frac{16}{5}+\frac95\\
\frac85+\frac{27}{5}
\end{pmatrix}
\]

\[
=
\begin{pmatrix}
\frac{25}{5}\\
\frac{35}{5}
\end{pmatrix}
=
\begin{pmatrix}
5\\
7
\end{pmatrix}
=b
\]

The result matches the original vector b.

### Final Answer

\[
\boxed{
x=
\begin{pmatrix}
\frac85\\
\frac95
\end{pmatrix}
}
\]

The solution is correct because substituting x into Ax = b gives the original vector b.
