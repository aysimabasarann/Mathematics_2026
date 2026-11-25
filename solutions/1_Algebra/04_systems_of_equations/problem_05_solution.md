### Exercise 5. Row Echelon Form and Number of Solutions

For the augmented matrix

$$
\begin{pmatrix}
1 & 2 & -1 & \mid & 3 \\
0 & 1 & 2 & \mid & 1 \\
0 & 0 & 0 & \mid & 0 \\
\end{pmatrix}
$$

determine the number of solutions and write them in parametric form. Explain how you know how many variables may be chosen freely.

---

## Solution

### 1. Determining the Number of Solutions

The given augmented matrix is already in row echelon form:

$$
\begin{pmatrix}
1 & 2 & -1 & \mid & 3 \\
0 & 1 & 2 & \mid & 1 \\
0 & 0 & 0 & \mid & 0 \\
\end{pmatrix}
$$

- The third row is $(0 \quad 0 \quad 0 \mid 0)$, which corresponds to the trivially satisfied identity $0 = 0$. Therefore, there is no contradiction and the system is **consistent**.
- There are $n = 3$ variables ($x_1, x_2, x_3$) and $r = 2$ nonzero rows (two pivots, located in columns 1 and 2).
- Because the number of pivots is less than the number of variables ($r < n$), the system has **infinitely many solutions**.

### 2. Number of Free Variables

The number of variables that can be chosen freely is determined by the difference between the total number of variables and the number of pivot columns (the rank of the matrix):

$$
\text{Number of free variables} = n - r = 3 - 2 = 1
$$

Since columns 1 and 2 contain leading pivots corresponding to the basic variables $x_1$ and $x_2$, column 3 has no pivot. Thus, $x_3$ is the **one free variable**.

### 3. Writing the Solutions in Parametric Form

Rewriting the non-trivial rows of the augmented matrix as a system of linear equations gives:

$$
\begin{cases}
x_1 + 2x_2 - x_3 = 3, \\
x_2 + 2x_3 = 1.
\end{cases}
$$

Assign a free parameter $t \in \mathbb{R}$ to the free variable:

$$
x_3 = t
$$

Substitute $x_3 = t$ into the second equation to express $x_2$ in terms of $t$:

$$
x_2 + 2t = 1 \implies x_2 = 1 - 2t
$$

Substitute both $x_2 = 1 - 2t$ and $x_3 = t$ into the first equation to find $x_1$:

$$
x_1 + 2(1 - 2t) - t = 3
$$

Simplifying the expression:

$$
x_1 + 2 - 4t - t = 3 \implies x_1 - 5t = 1 \implies x_1 = 1 + 5t
$$

Thus, the complete solution set in parametric form is:

$$
\begin{cases}
x_1 = 1 + 5t, \\
x_2 = 1 - 2t, \\
x_3 = t,
\end{cases}
\quad (t \in \mathbb{R})
$$
