 ### Exercise 3. Inconsistent System

Solve or show that the system is inconsistent:

$$
\begin{cases}
x+2y=3, \\
2x+4y=7.
\end{cases}
$$

Show how the contradiction appears in the matrix after elimination and interpret it in terms of equations.

---

## Solution

### 1. Gaussian Elimination on the Augmented Matrix

The augmented matrix corresponding to the system is

$$
\begin{pmatrix}
1 & 2 & \mid & 3 \\
2 & 4 & \mid & 7 \\
\end{pmatrix}
$$

To eliminate the entry below the pivot in the first column, apply the row operation $R_2 \leftarrow R_2 - 2R_1$:

$$
\begin{pmatrix}
1 & 2 & \mid & 3 \\
0 & 0 & \mid & 1 \\
\end{pmatrix}
$$

### 2. Contradiction in the Matrix and Equation Interpretation

After elimination, the second row of the augmented matrix is $(0 \quad 0 \mid 1)$, where all coefficients on the left-hand side are zero while the right-hand side entry is nonzero.

Translating this second row back into an algebraic equation gives

$$
0x + 0y = 1 \implies 0 = 1
$$

This is a logical contradiction because $0 = 1$ can never be satisfied for any real values of $x$ and $y$. Equivalently, multiplying the first equation $x + 2y = 3$ by $2$ requires $2x + 4y = 6$, which directly conflicts with the second equation $2x + 4y = 7$.

Therefore, the system is **inconsistent** and has no solution.

