
# Exercise 1 – Definition of the Inverse

## Solution

Given:

\[
A=
\begin{pmatrix}
2&1\\
1&1
\end{pmatrix},
\qquad
B=
\begin{pmatrix}
1&-1\\
-1&2
\end{pmatrix}
\]

We need to check whether \(B=A^{-1}\) without using an inverse formula.

### Step 1. Calculate AB

\[
AB=
\begin{pmatrix}
2&1\\
1&1
\end{pmatrix}
\begin{pmatrix}
1&-1\\
-1&2
\end{pmatrix}
\]

\[
=
\begin{pmatrix}
2-1&-2+2\\
1-1&-1+2
\end{pmatrix}
\]

\[
AB=
\begin{pmatrix}
1&0\\
0&1
\end{pmatrix}
=I
\]

### Step 2. Calculate BA

\[
BA=
\begin{pmatrix}
1&-1\\
-1&2
\end{pmatrix}
\begin{pmatrix}
2&1\\
1&1
\end{pmatrix}
\]

\[
=
\begin{pmatrix}
2-1&1-1\\
-2+2&-1+2
\end{pmatrix}
\]

\[
BA=
\begin{pmatrix}
1&0\\
0&1
\end{pmatrix}
=I
\]

### Step 3. Relate the result to the definition of the inverse

A matrix \(B\) is the inverse of \(A\) if:

\[
AB=BA=I
\]

Since both products are equal to the identity matrix, \(B\) is the inverse of \(A\).

### Final Answer

\[
\boxed{B=A^{-1}}
\]

The matrix \(B\) is the inverse of \(A\) because multiplying them in either order gives the identity matrix.
