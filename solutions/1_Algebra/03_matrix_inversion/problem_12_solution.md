### Exercise 12. Finding Inverses Without Starting from Scratch

It is known that

$$
A^{-1}=
\begin{pmatrix}
2 & -1 \\
-3 & 2 \\
\end{pmatrix}
$$

Without finding $A$, compute $(3A)^{-1}$, $(A^T)^{-1}$, and $(A^2)^{-1}$. Justify each result using the appropriate property.

---

## Solution

### 1. Computing $(3A)^{-1}$

**Property:** For any invertible matrix $A$ and nonzero scalar $c$, the inverse of a scalar multiple is given by:

$$
(cA)^{-1} = \frac{1}{c}A^{-1}
$$

Using this property with $c = 3$:

$$
(3A)^{-1} = \frac{1}{3}
\begin{pmatrix}
2 & -1 \\
-3 & 2 \\
\end{pmatrix}
$$

Multiplying by the scalar $\frac{1}{3}$:

$$
(3A)^{-1} =
\begin{pmatrix}
\frac{2}{3} & -\frac{1}{3} \\
-1 & \frac{2}{3} \\
\end{pmatrix}
$$

### 2. Computing $(A^T)^{-1}$

**Property:** The inverse of a transposed matrix is equal to the transpose of its inverse:

$$
(A^T)^{-1} = (A^{-1})^T
$$

Using this property, we transpose the given matrix $A^{-1}$ by swapping its rows and columns:

$$
(A^T)^{-1} =
\begin{pmatrix}
2 & -3 \\
-1 & 2 \\
\end{pmatrix}
$$

### 3. Computing $(A^2)^{-1}$

**Property:** The inverse of a matrix raised to a power is equal to the inverse matrix raised to that same power:

$$
(A^2)^{-1} = (A^{-1})^2
$$

Using this property, we compute the product $A^{-1}A^{-1}$:

$$
(A^2)^{-1} =
\begin{pmatrix}
2 & -1 \\
-3 & 2 \\
\end{pmatrix}
\begin{pmatrix}
2 & -1 \\
-3 & 2 \\
\end{pmatrix}
$$

Writing out the multiplication of entries:

$$
(A^2)^{-1} =
\begin{pmatrix}
(2)(2) + (-1)(-3) & (2)(-1) + (-1)(2) \\
(-3)(2) + (2)(-3) & (-3)(-1) + (2)(2) \\
\end{pmatrix}
$$

Simplifying the entries:

$$
(A^2)^{-1} =
\begin{pmatrix}
4 + 3 & -2 - 2 \\
-6 - 6 & 3 + 4 \\
\end{pmatrix}
$$

Evaluating the sums:

$$
(A^2)^{-1} =
\begin{pmatrix}
7 & -4 \\
-12 & 7 \\
\end{pmatrix}
$$
