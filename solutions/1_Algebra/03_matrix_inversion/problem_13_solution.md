
# Exercise 13 – Undoing a Composite Transformation

## Given

\[
S=
\begin{pmatrix}
2&0\\
0&1
\end{pmatrix},
\qquad
H=
\begin{pmatrix}
1&1\\
0&1
\end{pmatrix}
\]

Given:

\[
T=HS
\]

### 1. Describe the transformations

The matrix S represents nonuniform scaling. It stretches the x-coordinate by a factor of 2 while leaving the y-coordinate unchanged.

The matrix H represents a horizontal shear transformation. It adds the y-coordinate to the x-coordinate while keeping the y-coordinate unchanged.

### 2. First method: Compute T and then its inverse

Since:

\[
T=HS
\]

we calculate:

\[
T=
\begin{pmatrix}
1&1\\
0&1
\end{pmatrix}
\begin{pmatrix}
2&0\\
0&1
\end{pmatrix}
\]

\[
T=
\begin{pmatrix}
2&1\\
0&1
\end{pmatrix}
\]

Now calculate its determinant:

\[
\det(T)=2\cdot1-0\cdot1=2
\]

Using the inverse formula:

\[
T^{-1}=
\frac{1}{2}
\begin{pmatrix}
1&-1\\
0&2
\end{pmatrix}
\]

Therefore:

\[
\boxed{
T^{-1}=
\begin{pmatrix}
\frac12&-\frac12\\
0&1
\end{pmatrix}
}
\]

### 3. Second method: Use the inverse of a product

Using the property:

\[
(HS)^{-1}=S^{-1}H^{-1}
\]

First, calculate the individual inverses:

\[
S^{-1}=
\begin{pmatrix}
\frac12&0\\
0&1
\end{pmatrix}
\]

\[
H^{-1}=
\begin{pmatrix}
1&-1\\
0&1
\end{pmatrix}
\]

Now multiply:

\[
T^{-1}=S^{-1}H^{-1}
\]

\[
=
\begin{pmatrix}
\frac12&0\\
0&1
\end{pmatrix}
\begin{pmatrix}
1&-1\\
0&1
\end{pmatrix}
\]

\[
\boxed{
T^{-1}=
\begin{pmatrix}
\frac12&-\frac12\\
0&1
\end{pmatrix}
}
\]

Both methods give the same result.

### 4. Check the incorrect order

Now calculate:

\[
H^{-1}S^{-1}
\]

\[
=
\begin{pmatrix}
1&-1\\
0&1
\end{pmatrix}
\begin{pmatrix}
\frac12&0\\
0&1
\end{pmatrix}
\]

\[
\boxed{
H^{-1}S^{-1}=
\begin{pmatrix}
\frac12&-1\\
0&1
\end{pmatrix}
}
\]

This is different from the correct inverse:

\[
S^{-1}H^{-1}\neq H^{-1}S^{-1}
\]

Therefore, the order of matrix multiplication matters.

### 5. Conclusion

The correct inverse is:

\[
\boxed{
T^{-1}=
\begin{pmatrix}
\frac12&-\frac12\\
0&1
\end{pmatrix}
}
\]

When undoing a composition of operations, we must reverse the order of the operations.

Since T = HS, we first undo H and then undo S.

This is why:

\[
(HS)^{-1}=S^{-1}H^{-1}
\]
