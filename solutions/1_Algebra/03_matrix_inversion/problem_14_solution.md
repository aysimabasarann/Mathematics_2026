
# Exercise 14 – A Matrix That Is Its Own Inverse

## Given

Assume that a square matrix A satisfies:

\[
A^2=I
\]

We need to show that:

\[
A^{-1}=A
\]

### 1. Proof

By definition, the inverse of a matrix A is a matrix that satisfies:

\[
AA^{-1}=A^{-1}A=I
\]

We are given:

\[
A^2=I
\]

Since:

\[
A^2=A\cdot A=I
\]

the matrix A multiplied by itself gives the identity matrix.

Therefore, A satisfies the definition of its own inverse.

Hence:

\[
\boxed{A^{-1}=A}
\]

### 2. Give an example of a 2 × 2 matrix

Choose a matrix different from I and -I:

\[
A=
\begin{pmatrix}
0&1\\
1&0
\end{pmatrix}
\]

### 3. Verify by multiplication

Calculate A²:

\[
A^2=
\begin{pmatrix}
0&1\\
1&0
\end{pmatrix}
\begin{pmatrix}
0&1\\
1&0
\end{pmatrix}
\]

Multiplying the matrices:

\[
A^2=
\begin{pmatrix}
0\cdot0+1\cdot1&0\cdot1+1\cdot0\\
1\cdot0+0\cdot1&1\cdot1+0\cdot0
\end{pmatrix}
\]

\[
A^2=
\begin{pmatrix}
1&0\\
0&1
\end{pmatrix}
=I
\]

Therefore:

\[
\boxed{A^{-1}=A}
\]

### 4. Conclusion

The matrix A is its own inverse because multiplying it by itself gives the identity matrix.

This example satisfies the condition:

\[
A^2=I
\]

and is different from both I and -I.
