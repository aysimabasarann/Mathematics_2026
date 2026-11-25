### Exercise 12. A Parameter Revealed by a Row Operation

For

$$
A(t)=
\begin{pmatrix}
1 & 2 & 3 \\
2 & 4 & t \\
0 & 1 & 1 \\
\end{pmatrix}
$$

find the values of $t$ for which the matrix is not invertible.

Before computing the determinant, perform the operation

$$
R_2 \leftarrow R_2 - 2R_1
$$

and use the resulting structure. At the end, explain what special thing happens to the rows for the value of the parameter you found.

---

## Solution

### 1. Applying the Specified Row Operation

We begin by performing the row operation $R_2 \leftarrow R_2 - 2R_1$ on matrix $A(t)$:

$$
A_1 =
\begin{pmatrix}
1 & 2 & 3 \\
2 - 2(1) & 4 - 2(2) & t - 2(3) \\
0 & 1 & 1 \\
\end{pmatrix}
$$

Simplifying the entries of the second row:

$$
A_1 =
\begin{pmatrix}
1 & 2 & 3 \\
0 & 0 & t - 6 \\
0 & 1 & 1 \\
\end{pmatrix}
$$

### 2. Computing the Determinant and Finding $t$

Next, we swap rows $R_2$ and $R_3$ to put the matrix into upper-triangular form. Swapping two rows multiplies the determinant by $-1$:

$$
\det A(t) = - \det
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 1 \\
0 & 0 & t - 6 \\
\end{pmatrix}
$$

Since the resulting matrix is upper-triangular, its determinant is the product of its main diagonal entries:

$$
\det A(t) = - (1 \cdot 1 \cdot (t - 6)) = -(t - 6) = 6 - t
$$

A matrix is not invertible if and only if its determinant is zero. Setting $\det A(t) = 0$:

$$
6 - t = 0 \implies t = 6
$$

### 3. Explanation of the Row Structure for $t = 6$

When $t = 6$, the original matrix becomes:

$$
A(6) =
\begin{pmatrix}
1 & 2 & 3 \\
2 & 4 & 6 \\
0 & 1 & 1 \\
\end{pmatrix}
$$

For this specific value of the parameter, the second row $R_2 = (2, 4, 6)$ becomes an exact scalar multiple of the first row $R_1 = (1, 2, 3)$, since $R_2 = 2R_1$.

This linear dependence between the rows means the rows do not span full 3-dimensional space, causing the determinant to collapse to zero and rendering the matrix non-invertible.



