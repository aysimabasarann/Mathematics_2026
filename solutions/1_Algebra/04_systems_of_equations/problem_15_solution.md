### Exercise 15. Classifying Three Systems

For each of the following systems, perform only as much elimination as necessary to recognize its type:

**System 1**

$$
\begin{cases}
x+y=2, \\
x-y=0,
\end{cases}
$$

**System 2**

$$
\begin{cases}
x+y=2, \\
2x+2y=4,
\end{cases}
$$

**System 3**

$$
\begin{cases}
x+y=2, \\
2x+2y=5.
\end{cases}
$$

For each, justify the classification: one solution, infinitely many solutions, or no solution.

---

## Solution

### 1. System 1

We write the augmented matrix for System 1:

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
1 & -1 & \mid & 0 \\
\end{pmatrix}
$$

Apply the row operation $R_2 \leftarrow R_2 - R_1$ to eliminate the entry below the first pivot:

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
0 & -2 & \mid & -2 \\
\end{pmatrix}
$$

**Classification and Justification:** **Exactly one solution.** 
The reduced matrix is in row echelon form with $r = 2$ nonzero pivots (one in column 1 and one in column 2), matching the $n = 2$ unknowns. Because there are no contradictory rows and no free variables ($n - r = 0$), the system has a unique solution (specifically, $y = 1$ and $x = 1$).

### 2. System 2

We write the augmented matrix for System 2:

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
2 & 2 & \mid & 4 \\
\end{pmatrix}
$$

Apply the row operation $R_2 \leftarrow R_2 - 2R_1$:

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
0 & 0 & \mid & 0 \\
\end{pmatrix}
$$

**Classification and Justification:** **Infinitely many solutions.** 
The second row reduces completely to $(0 \quad 0 \mid 0)$, which corresponds to the true identity $0 = 0$, confirming the system is consistent. However, there is only $r = 1$ pivot for $n = 2$ unknowns, leaving $2 - 1 = 1$ free variable ($y = t \in \mathbb{R}$, $x = 2 - t$). Thus, infinitely many solutions exist.

### 3. System 3

We write the augmented matrix for System 3:

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
2 & 2 & \mid & 5 \\
\end{pmatrix}
$$

Apply the row operation $R_2 \leftarrow R_2 - 2R_1$:

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
0 & 0 & \mid & 1 \\
\end{pmatrix}
$$

**Classification and Justification:** **No solution (inconsistent).** 
After one elimination step, the second row becomes $(0 \quad 0 \mid 1)$, which translates to the false equation $0x + 0y = 1 \implies 0 = 1$. Since this contradiction can never be satisfied by any real numbers $x$ and $y$, the system has no solution.
