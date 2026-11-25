
# Exercise 10 – Inverse of a Diagonal Matrix

## Solution

Given:

\[
D=
\begin{pmatrix}
2&0&0\\
0&-3&0\\
0&0&5
\end{pmatrix}
\]

\[
E=
\begin{pmatrix}
2&0&0\\
0&0&0\\
0&0&5
\end{pmatrix}
\]

### Step 1. Determine which matrix is invertible

A diagonal matrix is invertible if all its diagonal entries are nonzero.

For matrix D, the diagonal entries are 2, -3 and 5.

Since none of them is zero, D is invertible.

For matrix E, one diagonal entry is zero.

Therefore, E is not invertible.

### Step 2. Find the inverse of D

To find the inverse of a diagonal matrix, take the reciprocal of each diagonal entry.

\[
D^{-1}=
\begin{pmatrix}
\frac{1}{2}&0&0\\
0&-\frac{1}{3}&0\\
0&0&\frac{1}{5}
\end{pmatrix}
\]

### Step 3. Check the result by multiplication

We multiply D by its inverse:

\[
DD^{-1}=
\begin{pmatrix}
2&0&0\\
0&-3&0\\
0&0&5
\end{pmatrix}
\begin{pmatrix}
\frac12&0&0\\
0&-\frac13&0\\
0&0&\frac15
\end{pmatrix}
\]

\[
=
\begin{pmatrix}
2\cdot\frac12&0&0\\
0&-3\cdot(-\frac13)&0\\
0&0&5\cdot\frac15
\end{pmatrix}
\]

\[
=
\begin{pmatrix}
1&0&0\\
0&1&0\\
0&0&1
\end{pmatrix}
=I
\]

### Conclusion

Matrix D is invertible, while matrix E is not invertible because it has a zero diagonal entry.

The inverse of D is:

\[
\boxed{
D^{-1}=
\begin{pmatrix}
\frac12&0&0\\
0&-\frac13&0\\
0&0&\frac15
\end{pmatrix}
}
\]

The multiplication confirms that \(DD^{-1}=I\).
