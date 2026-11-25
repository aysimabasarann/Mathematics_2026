
# Exercise 12 – Finding Inverses Without Starting from Scratch

## Given

\[
A^{-1}=
\begin{pmatrix}
2&-1\\
-3&2
\end{pmatrix}
\]

We need to compute:

\[
(3A)^{-1},\quad (A^T)^{-1},\quad (A^2)^{-1}
\]

### 1. Compute \((3A)^{-1}\)

Using the scalar inverse property:

\[
(3A)^{-1}=\frac{1}{3}A^{-1}
\]

\[
=\frac13
\begin{pmatrix}
2&-1\\
-3&2
\end{pmatrix}
\]

Therefore:

\[
\boxed{
(3A)^{-1}=
\begin{pmatrix}
\frac23&-\frac13\\
-1&\frac23
\end{pmatrix}
}
\]

### 2. Compute \((A^T)^{-1}\)

Using the transpose property:

\[
(A^T)^{-1}=(A^{-1})^T
\]

\[
=
\begin{pmatrix}
2&-1\\
-3&2
\end{pmatrix}^T
\]

Therefore:

\[
\boxed{
(A^T)^{-1}=
\begin{pmatrix}
2&-3\\
-1&2
\end{pmatrix}
}
\]

### 3. Compute \((A^2)^{-1}\)

Using the inverse of a product property:

\[
(AB)^{-1}=B^{-1}A^{-1}
\]

\[
(A^2)^{-1}=A^{-1}A^{-1}
\]

\[
=
\begin{pmatrix}
2&-1\\
-3&2
\end{pmatrix}
\begin{pmatrix}
2&-1\\
-3&2
\end{pmatrix}
\]

\[
=
\begin{pmatrix}
7&-4\\
-12&7
\end{pmatrix}
\]

Therefore:

\[
\boxed{
(A^2)^{-1}=
\begin{pmatrix}
7&-4\\
-12&7
\end{pmatrix}
}
\]

### Conclusion

The final answers are:

\[
(3A)^{-1}=
\begin{pmatrix}
\frac23&-\frac13\\
-1&\frac23
\end{pmatrix}
\]

\[
(A^T)^{-1}=
\begin{pmatrix}
2&-3\\
-1&2
\end{pmatrix}
\]

\[
(A^2)^{-1}=
\begin{pmatrix}
7&-4\\
-12&7
\end{pmatrix}
\]

All results are obtained using inverse properties without calculating the original matrix A.
