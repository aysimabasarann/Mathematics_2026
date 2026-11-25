
# Exercise 2 – Formula for a 2×2 Matrix

## Solution

Given:

\[
A=
\begin{pmatrix}
3&2\\
5&4
\end{pmatrix}
\]

### Step 1. Calculate the determinant

For a 2×2 matrix:

\[
\det(A)=ad-bc
\]

\[
\det(A)=(3)(4)-(2)(5)
\]

\[
=12-10=2
\]

Since the determinant is not zero, the inverse exists.

### Step 2. Apply the inverse formula

The inverse formula for a 2×2 matrix is:

\[
A^{-1}=\frac{1}{ad-bc}
\begin{pmatrix}
d&-b\\
-c&a
\end{pmatrix}
\]

Substituting the values:

\[
A^{-1}=\frac{1}{2}
\begin{pmatrix}
4&-2\\
-5&3
\end{pmatrix}
\]

Therefore:

\[
\boxed{
A^{-1}=
\begin{pmatrix}
2&-1\\
-\frac{5}{2}&\frac{3}{2}
\end{pmatrix}
}
\]

### Step 3. Verify the result

Multiply \(A\) by \(A^{-1}\):

\[
AA^{-1}=
\begin{pmatrix}
3&2\\
5&4
\end{pmatrix}
\begin{pmatrix}
2&-1\\
-\frac52&\frac32
\end{pmatrix}
\]

\[
=
\begin{pmatrix}
6-5&-3+3\\
10-10&-5+6
\end{pmatrix}
\]

\[
=
\begin{pmatrix}
1&0\\
0&1
\end{pmatrix}
=I
\]

### Final Answer

\[
\boxed{
A^{-1}=
\begin{pmatrix}
2&-1\\
-\frac52&\frac32
\end{pmatrix}
}
\]

The result is correct because multiplying the original matrix by its inverse gives the identity matrix.
