### Exercise 2. Gaussian Elimination — One Solution

Solve using Gaussian elimination:

$$
\begin{cases}
x+y+z=6, \\
2x-y+z=3, \\
x+2y-z=2.
\end{cases}
$$

After solving, substitute the result into all equations and check consistency.

---

## Solution

### 1. Setting Up the Augmented Matrix

The augmented matrix corresponding to the given system is

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 6 \\
2 & -1 & 1 & \mid & 3 \\
1 & 2 & -1 & \mid & 2 \\
\end{pmatrix}
$$

### 2. Forward Elimination

To eliminate the entries below the first pivot in column 1, perform the row operations $R_2 \leftarrow R_2 - 2R_1$ and $R_3 \leftarrow R_3 - R_1$:

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 6 \\
0 & -3 & -1 & \mid & -9 \\
0 & 1 & -2 & \mid & -4 \\
\end{pmatrix}
$$

Swap rows $R_2$ and $R_3$ ($R_2 \leftrightarrow R_3$) to get a pivot of $1$ in the second column:

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 6 \\
0 & 1 & -2 & \mid & -4 \\
0 & -3 & -1 & \mid & -9 \\
\end{pmatrix}
$$

To eliminate the entry below the second pivot in column 2, apply the row operation $R_3 \leftarrow R_3 + 3R_2$:

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 6 \\
0 & 1 & -2 & \mid & -4 \\
0 & 0 & -7 & \mid & -21 \\
\end{pmatrix}
$$

### 3. Back-Substitution

The matrix is now in row echelon form, which corresponds to the simplified system

$$
\begin{cases}
x + y + z = 6, \\
y - 2z = -4, \\
-7z = -21.
\end{cases}
$$

From the third equation, solve for $z$:

$$
-7z = -21 \implies z = 3
$$

Substitute $z = 3$ into the second equation to find $y$:

$$
y - 2(3) = -4 \implies y - 6 = -4 \implies y = 2
$$

Substitute $y = 2$ and $z = 3$ into the first equation to find $x$:

$$
x + 2 + 3 = 6 \implies x + 5 = 6 \implies x = 1
$$

Thus, the unique solution is $(x, y, z) = (1, 2, 3)$.

### 4. Verification of Consistency

Substitute $x = 1$, $y = 2$, and $z = 3$ back into each equation of the original system:

- **Equation 1:** $1 + 2 + 3 = 6$ (holds true).
- **Equation 2:** $2(1) - 2 + 3 = 2 - 2 + 3 = 3$ (holds true).
- **Equation 3:** $1 + 2(2) - 3 = 1 + 4 - 3 = 2$ (holds true).

Since all three equations are satisfied, the solution $(1, 2, 3)$ is verified.
