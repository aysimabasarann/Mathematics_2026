### Exercise 12. Homogeneous System

Solve

$$
\begin{cases}
x+2y-z=0, \\
2x+4y-2z=0, \\
x-y+2z=0.
\end{cases}
$$

Give all solutions in parametric form and explain why $(0,0,0)$ always satisfies a homogeneous system.

---

## Solution

### 1. Setting Up the Augmented Matrix

We write the homogeneous system as an augmented matrix:

$$
\begin{pmatrix}
1 & 2 & -1 & \mid & 0 \\
2 & 4 & -2 & \mid & 0 \\
1 & -1 & 2 & \mid & 0 \\
\end{pmatrix}
$$

### 2. Forward Elimination

To eliminate the entries below the first pivot in column 1, apply the row operations $R_2 \leftarrow R_2 - 2R_1$ and $R_3 \leftarrow R_3 - R_1$:

$$
\begin{pmatrix}
1 & 2 & -1 & \mid & 0 \\
0 & 0 & 0 & \mid & 0 \\
0 & -3 & 3 & \mid & 0 \\
\end{pmatrix}
$$

Swap rows $R_2$ and $R_3$ ($R_2 \leftrightarrow R_3$) to move the zero row to the bottom:

$$
\begin{pmatrix}
1 & 2 & -1 & \mid & 0 \\
0 & -3 & 3 & \mid & 0 \\
0 & 0 & 0 & \mid & 0 \\
\end{pmatrix}
$$

Divide the second row by $-3$ ($R_2 \leftarrow -\frac{1}{3}R_2$) to obtain a leading $1$:

$$
\begin{pmatrix}
1 & 2 & -1 & \mid & 0 \\
0 & 1 & -1 & \mid & 0 \\
0 & 0 & 0 & \mid & 0 \\
\end{pmatrix}
$$

### 3. Parametric Solution

The matrix is now in row echelon form, corresponding to the simplified system:

$$
\begin{cases}
x + 2y - z = 0, \\
y - z = 0.
\end{cases}
$$

The leading pivots are in columns 1 and 2 (for $x$ and $y$), leaving column 3 (for $z$) as a free variable. Let $z = t$, where $t \in \mathbb{R}$.

From the second equation, express $y$ in terms of $t$:

$$
y - t = 0 \implies y = t
$$

Substitute $y = t$ and $z = t$ into the first equation to find $x$:

$$
x + 2t - t = 0 \implies x + t = 0 \implies x = -t
$$

Thus, all solutions in parametric form are given by:

$$
\begin{cases}
x = -t, \\
y = t, \\
z = t,
\end{cases}
\quad (t \in \mathbb{R})
$$

### 4. Why $(0,0,0)$ Always Satisfies a Homogeneous System

A homogeneous linear system has the general matrix form $Ax = 0$, where every equation has a constant term equal to zero on the right-hand side:

$$
a_{i1}x_1 + a_{i2}x_2 + \dots + a_{in}x_n = 0
$$

When we substitute the zero vector $(x_1, x_2, \dots, x_n) = (0, 0, \dots, 0)$ into any linear equation without a nonzero constant term, every product $a_{ij} \cdot 0$ evaluates to $0$. Therefore, the left-hand side sums to $0$, which identically matches the right-hand side $0$ for every equation in the system. Consequently, the trivial solution $(0,0,0)$ is guaranteed to be a valid solution for every homogeneous system regardless of the coefficient matrix.
