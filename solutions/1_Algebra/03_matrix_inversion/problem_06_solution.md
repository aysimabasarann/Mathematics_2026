### Exercise 6. Solving a System Using the Inverse

Solve

$$
Ax=b,
$$

where

$$
A=
\begin{pmatrix}
2 & 1 \\
1 & 3 \\
\end{pmatrix},\qquad b=
\begin{pmatrix}
5 \\
7 \\
\end{pmatrix},
$$

using $x=A^{-1}b$. Then substitute the resulting vector back into the equation and check the result.

---

## Solution

### 1. Finding the Inverse Matrix $A^{-1}$

First, we compute the determinant of the $2 \times 2$ coefficient matrix $A$:

$$
\det A = (2)(3) - (1)(1) = 6 - 1 = 5
$$

Since $\det A = 5 \neq 0$, the matrix $A$ is invertible. Applying the $2 \times 2$ inverse formula yields:

$$
A^{-1} = \frac{1}{5}
\begin{pmatrix}
3 & -1 \\
-1 & 2 \\
\end{pmatrix}
$$

### 2. Computing the Solution $x = A^{-1}b$

Next, we multiply $A^{-1}$ on the left of the right-hand side vector $b$:

$$
\begin{aligned}
x &= A^{-1}b \\
  &= \frac{1}{5}
\begin{pmatrix}
3 & -1 \\
-1 & 2 \\
\end{pmatrix}
\begin{pmatrix}
5 \\
7 \\
\end{pmatrix} \\
  &= \frac{1}{5}
\begin{pmatrix}
(3)(5) + (-1)(7) \\
(-1)(5) + (2)(7) \\
\end{pmatrix} \\
  &= \frac{1}{5}
\begin{pmatrix}
15 - 7 \\
-5 + 14 \\
\end{pmatrix} \\
  &= \frac{1}{5}
\begin{pmatrix}
8 \\
9 \\
\end{pmatrix}
=
\begin{pmatrix}
\frac{8}{5} \\
\frac{9}{5} \\
\end{pmatrix}
\end{aligned}
$$

### 3. Verification by Substitution

To check the solution, we substitute the resulting vector back into the original equation $Ax = b$:

$$
\begin{aligned}
Ax &=
\begin{pmatrix}
2 & 1 \\
1 & 3 \\
\end{pmatrix}
\begin{pmatrix}
\frac{8}{5} \\
\frac{9}{5} \\
\end{pmatrix} \\
   &=
\begin{pmatrix}
2\left(\frac{8}{5}\right) + 1\left(\frac{9}{5}\right) \\
1\left(\frac{8}{5}\right) + 3\left(\frac{9}{5}\right) \\
\end{pmatrix} \\
   &=
\begin{pmatrix}
\frac{16 + 9}{5} \\
\frac{8 + 27}{5} \\
\end{pmatrix} \\
   &=
\begin{pmatrix}
\frac{25}{5} \\
\frac{35}{5} \\
\end{pmatrix}
=
\begin{pmatrix}
5 \\
7 \\
\end{pmatrix}
= b
\end{aligned}
$$

Since $Ax = b$ holds, the solution $x = (8/5, 9/5)^T$ is verified.


