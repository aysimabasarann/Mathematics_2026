
# Exercise 11 – Parameter and Invertibility

## Solution

Given:

\[
A(t)=
\begin{pmatrix}
1&t\\
t&1
\end{pmatrix}
\]

### Step 1. Find the determinant

A matrix is invertible if and only if its determinant is not zero.

\[
\det A(t)=1\cdot1-t\cdot t
\]

\[
\det A(t)=1-t^2
\]

For the matrix to be invertible:

\[
1-t^2\neq0
\]

\[
t^2\neq1
\]

\[
t\neq\pm1
\]

Therefore, the matrix is invertible for:

\[
\boxed{t\neq-1,\quad t\neq1}
\]

### Step 2. Find the inverse formula

For a 2×2 matrix:

\[
A=
\begin{pmatrix}
a&b\\
c&d
\end{pmatrix}
\]

the inverse formula is:

\[
A^{-1}=\frac{1}{ad-bc}
\begin{pmatrix}
d&-b\\
-c&a
\end{pmatrix}
\]

Applying this formula:

\[
A(t)^{-1}
=
\frac{1}{1-t^2}
\begin{pmatrix}
1&-t\\
-t&1
\end{pmatrix}
\]

Thus:

\[
\boxed{
A(t)^{-1}
=
\frac{1}{1-t^2}
\begin{pmatrix}
1&-t\\
-t&1
\end{pmatrix},
\quad t\neq\pm1
}
\]

### Step 3. Explain the excluded values

When \(t=1\):

\[
A(1)=
\begin{pmatrix}
1&1\\
1&1
\end{pmatrix}
\]

The two rows are identical, so the determinant is zero.

When \(t=-1\):

\[
A(-1)=
\begin{pmatrix}
1&-1\\
-1&1
\end{pmatrix}
\]

The second row is the negative of the first row, so the determinant is zero.

In both cases, the matrix is not invertible.

The inverse formula is undefined because its denominator becomes zero:

\[
1-t^2=0
\]

### Conclusion

The matrix is invertible for all real values of \(t\) except:

\[
\boxed{t=-1,\quad t=1}
\]

The inverse does not exist at these excluded values because the determinant is zero.
