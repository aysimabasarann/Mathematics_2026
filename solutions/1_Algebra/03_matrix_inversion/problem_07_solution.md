### Exercise 7. Inverse of a Product

For

$$
A=
\begin{pmatrix}
1 & 1 \\
0 & 1 \\
\end{pmatrix},\qquad B=
\begin{pmatrix}
2 & 0 \\
0 & 3 \\
\end{pmatrix}
$$

compute $(AB)^{-1}$ and $B^{-1}A^{-1}$. Check that the results are the same and explain the meaning of the reversed order.

---

## Solution

### 1. Computing $(AB)^{-1}$

First, we compute the product matrix $AB$:

$$
AB =
\begin{pmatrix}
1 & 1 \\
0 & 1 \\
\end{pmatrix}
\begin{pmatrix}
2 & 0 \\
0 & 3 \\
\end{pmatrix}
$$

Writing out the multiplication of entries:

$$
AB =
\begin{pmatrix}
(1)(2) + (1)(0) & (1)(0) + (1)(3) \\
(0)(2) + (1)(0) & (0)(0) + (1)(3) \\
\end{pmatrix}
$$

Simplifying the entries:

$$
AB =
\begin{pmatrix}
2 + 0 & 0 + 3 \\
0 + 0 & 0 + 3 \\
\end{pmatrix}
=
\begin{pmatrix}
2 & 3 \\
0 & 3 \\
\end{pmatrix}
$$

Next, we compute the inverse of $AB$ using the $2 \times 2$ inverse formula. The determinant is:

$$
\det(AB) = (2)(3) - (3)(0) = 6
$$

Applying the formula:

$$
(AB)^{-1} = \frac{1}{6}
\begin{pmatrix}
3 & -3 \\
0 & 2 \\
\end{pmatrix}
$$

Multiplying by the scalar $\frac{1}{6}$:

$$
(AB)^{-1} =
\begin{pmatrix}
\frac{3}{6} & -\frac{3}{6} \\
0 & \frac{2}{6} \\
\end{pmatrix}
=
\begin{pmatrix}
\frac{1}{2} & -\frac{1}{2} \\
0 & \frac{1}{3} \\
\end{pmatrix}
$$

### 2. Computing $B^{-1}A^{-1}$

First, we find the individual inverses $A^{-1}$ and $B^{-1}$ using the $2 \times 2$ formula:

For matrix $A$, since $\det A = (1)(1) - (1)(0) = 1$:

$$
A^{-1} =
\begin{pmatrix}
1 & -1 \\
0 & 1 \\
\end{pmatrix}
$$

For matrix $B$, since $\det B = (2)(3) - (0)(0) = 6$:

$$
B^{-1} = \frac{1}{6}
\begin{pmatrix}
3 & 0 \\
0 & 2 \\
\end{pmatrix}
=
\begin{pmatrix}
\frac{3}{6} & 0 \\
0 & \frac{2}{6} \\
\end{pmatrix}
=
\begin{pmatrix}
\frac{1}{2} & 0 \\
0 & \frac{1}{3} \\
\end{pmatrix}
$$

Now, we compute the product $B^{-1}A^{-1}$:

$$
B^{-1}A^{-1} =
\begin{pmatrix}
\frac{1}{2} & 0 \\
0 & \frac{1}{3} \\
\end{pmatrix}
\begin{pmatrix}
1 & -1 \\
0 & 1 \\
\end{pmatrix}
$$

Writing out the multiplication:

$$
B^{-1}A^{-1} =
\begin{pmatrix}
\left(\frac{1}{2}\right)(1) + (0)(0) & \left(\frac{1}{2}\right)(-1) + (0)(1) \\
(0)(1) + \left(\frac{1}{3}\right)(0) & (0)(-1) + \left(\frac{1}{3}\right)(1) \\
\end{pmatrix}
$$

Simplifying the entries:

$$
B^{-1}A^{-1} =
\begin{pmatrix}
\frac{1}{2} + 0 & -\frac{1}{2} + 0 \\
0 + 0 & 0 + \frac{1}{3} \\
\end{pmatrix}
=
\begin{pmatrix}
\frac{1}{2} & -\frac{1}{2} \\
0 & \frac{1}{3} \\
\end{pmatrix}
$$

### 3. Comparison and Meaning of the Reversed Order

Comparing our two computations, we find that:

$$
(AB)^{-1} = B^{-1}A^{-1}
$$

**Meaning of the reversed order:** Matrix multiplication represents the composition of linear transformations. When matrix $A$ is applied followed by matrix $B$, the combined transformation is represented by $AB$. To undo this composite operation, we must reverse the steps in the exact opposite order: we must first undo $B$ (by applying $B^{-1}$), and then undo $A$ (by applying $A^{-1}$). Hence, the inverse of a product is the product of the inverses in reverse order.







 










 




 












