### Exercise 15. Two Methods for Solving the Same System

For

$$
A=
\begin{pmatrix}
2 & 1 \\
1 & 3 \\
\end{pmatrix},\qquad b=
\begin{pmatrix}
7 \\
8 \\
\end{pmatrix}
$$

solve $Ax=b$ in two ways:

1. using $A^{-1}b$,
2. using Gaussian elimination.

Compare both solutions, the number of essential steps, and state which method was simpler in this example.

---

## Solution

### 1. Solving Using $x = A^{-1}b$

First, we compute the determinant of the coefficient matrix $A$:

$$
\det A = (2)(3) - (1)(1) = 6 - 1 = 5
$$

Since $\det A = 5 \neq 0$, the matrix $A$ is invertible. Applying the $2 \times 2$ inverse formula gives:

$$
A^{-1} = \frac{1}{5}
\begin{pmatrix}
3 & -1 \\
-1 & 2 \\
\end{pmatrix}
$$

Next, we compute $x = A^{-1}b$:

$$
x = \frac{1}{5}
\begin{pmatrix}
3 & -1 \\
-1 & 2 \\
\end{pmatrix}
\begin{pmatrix}
7 \\
8 \\
\end{pmatrix}
$$

Writing out the matrix multiplication:

$$
x = \frac{1}{5}
\begin{pmatrix}
(3)(7) + (-1)(8) \\
(-1)(7) + (2)(8) \\
\end{pmatrix}
$$

Simplifying the entries:

$$
x = \frac{1}{5}
\begin{pmatrix}
21 - 8 \\
-7 + 16 \\
\end{pmatrix}
$$

Evaluating the sums:

$$
x = \frac{1}{5}
\begin{pmatrix}
13 \\
9 \\
\end{pmatrix}
$$

Distributing the scalar $\frac{1}{5}$:

$$
x =
\begin{pmatrix}
\frac{13}{5} \\
\frac{9}{5} \\
\end{pmatrix}
$$

### 2. Solving Using Gaussian Elimination

We set up the augmented matrix $[A \mid b]$:

$$
\begin{pmatrix}
2 & 1 & \mid & 7 \\
1 & 3 & \mid & 8 \\
\end{pmatrix}
$$

**Step 1:** Swap rows $R_1$ and $R_2$ ($R_1 \leftrightarrow R_2$) to place a leading $1$ in the top-left pivot position:

$$
\begin{pmatrix}
1 & 3 & \mid & 8 \\
2 & 1 & \mid & 7 \\
\end{pmatrix}
$$

**Step 2:** Eliminate the entry below the pivot in the first column by applying $R_2 \leftarrow R_2 - 2R_1$:

$$
\begin{pmatrix}
1 & 3 & \mid & 8 \\
0 & -5 & \mid & -9 \\
\end{pmatrix}
$$

From the second row, we obtain the equation for $x_2$:

$$
-5x_2 = -9 \implies x_2 = \frac{9}{5}
$$

Substituting $x_2 = \frac{9}{5}$ back into the first row equation $x_1 + 3x_2 = 8$:

$$
x_1 + 3\left(\frac{9}{5}\right) = 8
$$

Solving for $x_1$:

$$
x_1 = 8 - \frac{27}{5} = \frac{40 - 27}{5} = \frac{13}{5}
$$

Thus, the solution vector is:

$$
x =
\begin{pmatrix}
\frac{13}{5} \\
\frac{9}{5} \\
\end{pmatrix}
$$

### 3. Comparison of the Two Methods

Both methods yield the exact same unique solution: $x_1 = \frac{13}{5}$ and $x_2 = \frac{9}{5}$.

- **Number of essential steps:** 
  - The inverse method required computing the determinant, forming the adjugate matrix, multiplying by the scalar $\frac{1}{5}$, and performing a matrix-vector multiplication (4 main steps).
  - Gaussian elimination required a single row swap, one row elimination step, and back-substitution (3 main steps).

- **Which method was simpler:** In this example, **Gaussian elimination** was slightly simpler and more direct for solving a single system because it avoided computing the full inverse matrix $A^{-1}$ upfront. However, if we needed to solve $Ax = b$ repeatedly for many different right-hand side vectors $b$, finding $A^{-1}$ once would become the more efficient approach.


