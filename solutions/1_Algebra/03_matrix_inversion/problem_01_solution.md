### Exercise 1. Definition of the Inverse

For

$$
A=
\begin{pmatrix}
2 & 1 \\
1 & 1 \\
\end{pmatrix},\qquad B=
\begin{pmatrix}
1 & -1 \\
-1 & 2 \\
\end{pmatrix}
$$

check, without using a formula, whether $B=A^{-1}$. Compute $AB$ and $BA$ and relate the result to the definition of the inverse.

---

## Solution

### 1. Computing the Products $AB$ and $BA$

To check whether $B$ is the inverse of $A$ without using an explicit inverse formula, we compute the matrix products $AB$ and $BA$.

First, we compute the product $AB$:

$$
AB =
\begin{pmatrix}
2 & 1 \\
1 & 1 \\
\end{pmatrix}
\begin{pmatrix}
1 & -1 \\
-1 & 2 \\
\end{pmatrix}
=
\begin{pmatrix}
(2)(1) + (1)(-1) & (2)(-1) + (1)(2) \\
(1)(1) + (1)(-1) & (1)(-1) + (1)(2) \\
\end{pmatrix}
=
\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix}
= I
$$

Next, we compute the product $BA$:

$$
BA =
\begin{pmatrix}
1 & -1 \\
-1 & 2 \\
\end{pmatrix}
\begin{pmatrix}
2 & 1 \\
1 & 1 \\
\end{pmatrix}
=
\begin{pmatrix}
(1)(2) + (-1)(1) & (1)(1) + (-1)(1) \\
(-1)(2) + (2)(1) & (-1)(1) + (2)(1) \\
\end{pmatrix}
=
\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix}
= I
$$

### 2. Relation to the Definition of the Inverse

By definition, a square matrix $B$ is the inverse of a square matrix $A$ (denoted as $B = A^{-1}$) if and only if multiplying them in either order yields the identity matrix $I$:

$$
AB = BA = I
$$

Since both $AB = I$ and $BA = I$ hold true for the given matrices, we conclude without any formula that $B = A^{-1}$.



