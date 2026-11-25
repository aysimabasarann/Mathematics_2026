
# Exercise 8 – Inverse of a Transformation

## Solution

Given:

\[
S=
\begin{pmatrix}
2&0\\
0&\frac12
\end{pmatrix}
\]

### Step 1. Find the inverse matrix

For a diagonal matrix, we take the reciprocal of each diagonal entry.

Therefore:

\[
S^{-1}=
\begin{pmatrix}
\frac12&0\\
0&2
\end{pmatrix}
\]

### Step 2. Geometrical Explanation

The matrix S describes a scaling transformation of the plane.

- The x-coordinate is multiplied by 2.
- The y-coordinate is multiplied by 1/2.

The inverse transformation reverses these changes:

- The x-coordinate is multiplied by 1/2.
- The y-coordinate is multiplied by 2.

Thus, S⁻¹ undoes the original scaling transformation.

### Step 3. Check Using a Simple Vector

Choose:

\[
v=
\begin{pmatrix}
1\\
2
\end{pmatrix}
\]

First, apply S:

\[
Sv=
\begin{pmatrix}
2&0\\
0&\frac12
\end{pmatrix}
\begin{pmatrix}
1\\
2
\end{pmatrix}
=
\begin{pmatrix}
2\\
1
\end{pmatrix}
\]

Now apply S⁻¹:

\[
S^{-1}
\begin{pmatrix}
2\\
1
\end{pmatrix}
=
\begin{pmatrix}
\frac12&0\\
0&2
\end{pmatrix}
\begin{pmatrix}
2\\
1
\end{pmatrix}
=
\begin{pmatrix}
1\\
2
\end{pmatrix}
\]

We obtain the original vector.

Therefore:

\[
\boxed{S^{-1}Sv=v}
\]

### Conclusion

The inverse transformation reverses the scaling performed by S.

Applying S and then S⁻¹ returns every vector to its original position.

\[
\boxed{SS^{-1}=S^{-1}S=I}
\]
