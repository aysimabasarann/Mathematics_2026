### Exercise 4. Infinitely Many Solutions

Solve

$$
\begin{cases}
x+y+z=2, \\
2x+2y+2z=4, \\
x-y+z=0.
\end{cases}
$$

Give the solution in parametric form, identify a free variable, and for one chosen parameter value check that the resulting point really satisfies the system.

---

## Solution

### 1. Setting Up the Augmented Matrix

The augmented matrix corresponding to the given system is

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 2 \\
2 & 2 & 2 & \mid & 4 \\
1 & -1 & 1 & \mid & 0 \\
\end{pmatrix}
$$

### 2. Forward Elimination

To eliminate entries in the first column, apply the row operations $R_2 \leftarrow R_2 - 2R_1$ and $R_3 \leftarrow R_3 - R_1$:

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 2 \\
0 & 0 & 0 & \mid & 0 \\
0 & -2 & 0 & \mid & -2 \\
\end{pmatrix}
$$

Swap rows $R_2$ and $R_3$ ($R_2 \leftrightarrow R_3$) to place the non-zero row above the zero row:

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 2 \\
0 & -2 & 0 & \mid & -2 \\
0 & 0 & 0 & \mid & 0 \\
\end{pmatrix}
$$

Multiply the second row by $-\frac{1}{2}$ ($R_2 \leftarrow -\frac{1}{2}R_2$) to get a leading $1$ as a pivot:

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 2 \\
0 & 1 & 0 & \mid & 1 \\
0 & 0 & 0 & \mid & 0 \\
\end{pmatrix}
$$

### 3. Parametric Solution

The matrix is now in row echelon form, corresponding to the simplified system

$$
\begin{cases}
x + y + z = 2, \\
y = 1, \\
0 = 0.
\end{cases}
$$

Here, the variables $x$ and $y$ correspond to pivot columns, while $z$ is a free variable (let $z = t$, where $t \in \mathbb{R}$).

From the second equation, we already have $y = 1$. Substituting $y = 1$ and $z = t$ into the first equation:

$$
x + 1 + t = 2 \implies x = 1 - t
$$

Thus, the solutions in parametric form are:

$$
\begin{cases}
x = 1 - t, \\
y = 1, \\
z = t,
\end{cases}
\quad (t \in \mathbb{R})
$$

### 4. Verification for a Chosen Parameter Value

Let us choose the parameter value $t = 2$. The resulting point is:

$$
(x, y, z) = (1 - 2, 1, 2) = (-1, 1, 2)
$$

Substitute these values into each equation of the original system:

- **Equation 1:** $(-1) + 1 + 2 = 2$ (holds true).
- **Equation 2:** $2(-1) + 2(1) + 2(2) = -2 + 2 + 4 = 4$ (holds true).
- **Equation 3:** $(-1) - (1) + 2 = -2 + 2 = 0$ (holds true).

Since the point satisfies all equations, the parametric solution is verified.
