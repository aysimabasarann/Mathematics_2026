### Exercise 8. Two Systems with the Same Coefficient Matrix

Solve by elimination the two systems

$$
\begin{cases}
2x+y=5, \\
x-y=1,
\end{cases}
$$

$$
\begin{cases}
2x+y=1, \\
x-y=4.
\end{cases}
$$

Compare the successive elimination steps. Which part of the calculation is the same in both cases, and why?

---

## Solution

### 1. Solving the First System

We write the augmented matrix for the first system:

$$
\begin{pmatrix}
2 & 1 & \mid & 5 \\
1 & -1 & \mid & 1 \\
\end{pmatrix}
$$

Swap rows $R_1$ and $R_2$ ($R_1 \leftrightarrow R_2$) to place a leading $1$ in the top-left pivot position:

$$
\begin{pmatrix}
1 & -1 & \mid & 1 \\
2 & 1 & \mid & 5 \\
\end{pmatrix}
$$

Eliminate the entry below the pivot in the first column by applying the row operation $R_2 \leftarrow R_2 - 2R_1$:

$$
\begin{pmatrix}
1 & -1 & \mid & 1 \\
0 & 3 & \mid & 3 \\
\end{pmatrix}
$$

Divide the second row by $3$ ($R_2 \leftarrow \frac{1}{3}R_2$):

$$
\begin{pmatrix}
1 & -1 & \mid & 1 \\
0 & 1 & \mid & 1 \\
\end{pmatrix}
$$

From the second row, we read $y = 1$. Substituting $y = 1$ back into the first row equation $x - y = 1$ gives:

$$
x - 1 = 1 \implies x = 2
$$

Thus, the unique solution to the first system is $(x, y) = (2, 1)$.

### 2. Solving the Second System

We write the augmented matrix for the second system:

$$
\begin{pmatrix}
2 & 1 & \mid & 1 \\
1 & -1 & \mid & 4 \\
\end{pmatrix}
$$

Swap rows $R_1$ and $R_2$ ($R_1 \leftrightarrow R_2$):

$$
\begin{pmatrix}
1 & -1 & \mid & 4 \\
2 & 1 & \mid & 1 \\
\end{pmatrix}
$$

Eliminate the entry below the pivot in the first column by applying the identical row operation $R_2 \leftarrow R_2 - 2R_1$:

$$
\begin{pmatrix}
1 & -1 & \mid & 4 \\
0 & 3 & \mid & -7 \\
\end{pmatrix}
$$

Divide the second row by $3$ ($R_2 \leftarrow \frac{1}{3}R_2$):

$$
\begin{pmatrix}
1 & -1 & \mid & 4 \\
0 & 1 & \mid & -\frac{7}{3} \\
\end{pmatrix}
$$

From the second row, we have $y = -\frac{7}{3}$. Substituting this into the first row equation $x - y = 4$ gives:

$$
x - \left(-\frac{7}{3}\right) = 4 \implies x + \frac{7}{3} = 4 \implies x = \frac{12 - 7}{3} = \frac{5}{3}
$$

Thus, the unique solution to the second system is $(x, y) = \left(\frac{5}{3}, -\frac{7}{3}\right)$.

### 3. Comparison of Elimination Steps

- **What is identical:** The exact sequence of elementary row operations ($R_1 \leftrightarrow R_2$, followed by $R_2 \leftarrow R_2 - 2R_1$, and finally $R_2 \leftarrow \frac{1}{3}R_2$) and all resulting entries on the left-hand side (the coefficient columns) are completely identical in both systems.
- **What differs:** Only the numerical values in the augmented right-hand side column change at each step, leading to different final values for $x$ and $y$.
- **Why this happens:** The choice of pivots and the multipliers needed to eliminate entries below them depend exclusively on the entries of the coefficient matrix $A$. Since both systems share the exact same coefficient matrix $A = \begin{pmatrix} 2 & 1 \\ 1 & -1 \end{pmatrix}$, the reduction process on the left side is completely independent of the right-hand side vector $b$.
