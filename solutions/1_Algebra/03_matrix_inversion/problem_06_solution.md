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

First, we compute the determinant of the coefficient matrix $A$:

$$
\det A = (2)(3) - (1)(1) = 6 - 1 = 5
$$

Since $\det A = 5 \neq 0$, the matrix $A$ is invertible. Using the $2 \times 2$ inverse formula, we obtain:

$$
A^{-1} = \frac{1}{5}
\begin{pmatrix}
3 & -1 \\
-1 & 2 \\
\end{pmatrix}
$$

### 2. Computing the Solution $x = A^{-1}b$

We compute the solution vector $x$ by multiplying $A^{-1}$ by $b$:

$$
x = \frac{1}{5}
\begin{pmatrix}
3 & -1 \\
-1 & 2 \\
\end{pmatrix}
\begin{pmatrix}
5 \\
7 \\
\end{pmatrix}
$$

Multiplying the matrices inside:

$$
x = \frac{1}{5}
\begin{pmatrix}
(3)(5) + (-1)(7) \\
(-1)(5) + (2)(7) \\
\end{pmatrix}
$$

Evaluating the arithmetic in each entry:

$$
x = \frac{1}{5}
\begin{pmatrix}
15 - 7 \\
-5 + 14 \\
\end{pmatrix}
$$

Simplifying to a single column vector:

$$
x = \frac{1}{5}
\begin{pmatrix}
8 \\
9 \\
\end{pmatrix}
$$

Multiplying by the scalar $\frac{1}{5}$:

$$
x =
\begin{pmatrix}
\frac{8}{5} \\
\frac{9}{5} \\
\end{pmatrix}
$$

### 3. Verification by Substitution

To check the solution, we compute $Ax$ step by step. First, substitute the vectors:

$$
Ax =
\begin{pmatrix}
2 & 1 \\
1 & 3 \\
\end{pmatrix}
\begin{pmatrix}
\frac{8}{5} \\
\frac{9}{5} \\
\end{pmatrix}
$$

Write out the matrix multiplication:

$$
Ax =
\begin{pmatrix}
2\left(\frac{8}{5}\right) + 1\left(\frac{9}{5}\right) \\
1\left(\frac{8}{5}\right) + 3\left(\frac{9}{5}\right) \\
\end{pmatrix}
$$

Perform the multiplications:

$$
Ax =
\begin{pmatrix}
\frac{16}{5} + \frac{9}{5} \\
\frac{8}{5} + \frac{27}{5} \\
\end{pmatrix}
$$

Add the fractions:

$$
Ax =
\begin{pmatrix}
\frac{25}{5} \\
\frac{35}{5} \\
\end{pmatrix}
$$

Simplify the result:

$$
Ax =
\begin{pmatrix}
5 \\
7 \\
\end{pmatrix}
= b
$$

Since $Ax = b$ holds true, the solution is verified.
 






