
# Exercise 9 – Matrix Equation

## Solution

Given:

\[
A=
\begin{pmatrix}
1&2\\
0&1
\end{pmatrix},
\qquad
B=
\begin{pmatrix}
3&1\\
2&4
\end{pmatrix}
\]

We need to solve:

\[
AX=B
\]

### Step 1. Find the inverse of A

First, calculate the inverse of A:

\[
A^{-1}=
\begin{pmatrix}
1&-2\\
0&1
\end{pmatrix}
\]

### Step 2. Solve for X

Since A is on the left side of X, we multiply both sides by \(A^{-1}\) on the left.

\[
A^{-1}AX=A^{-1}B
\]

\[
IX=A^{-1}B
\]

Therefore:

\[
X=A^{-1}B
\]

Substitute the matrices:

\[
X=
\begin{pmatrix}
1&-2\\
0&1
\end{pmatrix}
\begin{pmatrix}
3&1\\
2&4
\end{pmatrix}
\]

Multiplying:

\[
X=
\begin{pmatrix}
3-4&1-8\\
2&4
\end{pmatrix}
\]

Thus:

\[
\boxed{
X=
\begin{pmatrix}
-1&-7\\
2&4
\end{pmatrix}
}
\]

### Step 3. Check the Result

We verify the answer by computing AX:

\[
AX=
\begin{pmatrix}
1&2\\
0&1
\end{pmatrix}
\begin{pmatrix}
-1&-7\\
2&4
\end{pmatrix}
\]

\[
=
\begin{pmatrix}
-1+4&-7+8\\
2&4
\end{pmatrix}
\]

\[
=
\begin{pmatrix}
3&1\\
2&4
\end{pmatrix}
=B
\]

### Conclusion

The solution is:

\[
\boxed{
X=
\begin{pmatrix}
-1&-7\\
2&4
\end{pmatrix}
}
\]

We multiply by \(A^{-1}\) on the left because A is on the left side of X. The verification confirms that AX = B.
