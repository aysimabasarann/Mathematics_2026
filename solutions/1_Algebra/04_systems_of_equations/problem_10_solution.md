### Exercise 10. A Polynomial Through Three Points

Find a polynomial $p(x)=ax^2+bx+c$ whose graph passes through $(0,1)$, $(1,3)$, and $(2,9)$. Reduce the problem to a system of equations and check the result by substituting all three points.

---

## Solution

### 1. Setting Up the System of Linear Equations

For the graph of $p(x) = ax^2 + bx + c$ to pass through a point $(x_0, y_0)$, we must have $p(x_0) = y_0$. Substituting each of the three given points produces a linear equation in the unknown coefficients $a$, $b$, and $c$:

- **Point $(0, 1)$:** $p(0) = a(0)^2 + b(0) + c = 1 \implies c = 1$
- **Point $(1, 3)$:** $p(1) = a(1)^2 + b(1) + c = 3 \implies a + b + c = 3$
- **Point $(2, 9)$:** $p(2) = a(2)^2 + b(2) + c = 9 \implies 4a + 2b + c = 9$

This gives the following system of three linear equations:

$$
\begin{cases}
c = 1, \\
a + b + c = 3, \\
4a + 2b + c = 9.
\end{cases}
$$

### 2. Solving the System via Gaussian Elimination

Ordering the variables as $(a, b, c)$, we write the augmented matrix of the system:

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 3 \\
4 & 2 & 1 & \mid & 9 \\
0 & 0 & 1 & \mid & 1 \\
\end{pmatrix}
$$

To eliminate the entry below the pivot in the first column, apply the row operation $R_2 \leftarrow R_2 - 4R_1$:

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 3 \\
0 & -2 & -3 & \mid & -3 \\
0 & 0 & 1 & \mid & 1 \\
\end{pmatrix}
$$

The matrix is now in row echelon form. We solve for the coefficients using back-substitution:

From the third row, we have:

$$
c = 1
$$

Substitute $c = 1$ into the second row equation $-2b - 3c = -3$:

$$
-2b - 3(1) = -3 \implies -2b = 0 \implies b = 0
$$

Substitute $b = 0$ and $c = 1$ into the first row equation $a + b + c = 3$:

$$
a + 0 + 1 = 3 \implies a = 2
$$

Thus, the coefficients are $a = 2$, $b = 0$, and $c = 1$, which gives the quadratic polynomial:

$$
p(x) = 2x^2 + 1
$$

### 3. Verification by Substituting All Three Points

We evaluate $p(x) = 2x^2 + 1$ at each given $x$-coordinate to confirm it passes through all three points:

- **At $x = 0$:** $p(0) = 2(0)^2 + 1 = 1$, matching $(0, 1)$.
- **At $x = 1$:** $p(1) = 2(1)^2 + 1 = 2 + 1 = 3$, matching $(1, 3)$.
- **At $x = 2$:** $p(2) = 2(2)^2 + 1 = 8 + 1 = 9$, matching $(2, 9)$.

All three points lie on the graph of $p(x) = 2x^2 + 1$, verifying the solution.
