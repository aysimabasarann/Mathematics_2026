### Exercise 13. Does Every Equation Add New Information?

Consider the system

$$
x_1+x_2=10,\qquad x_2+x_3=8,\qquad x_1-x_3=2.
$$

Solve it and check whether all three equations are independently necessary to describe the solution set. If one follows from the others, show this by calculation.

---

## Solution

### 1. Solving the System via Gaussian Elimination

We write the system as a set of three linear equations:

$$
\begin{cases}
x_1 + x_2 = 10, \\
x_2 + x_3 = 8, \\
x_1 - x_3 = 2.
\end{cases}
$$

Form the corresponding augmented matrix:

$$
\begin{pmatrix}
1 & 1 & 0 & \mid & 10 \\
0 & 1 & 1 & \mid & 8 \\
1 & 0 & -1 & \mid & 2 \\
\end{pmatrix}
$$

To eliminate the entry below the pivot in the first column, apply the row operation $R_3 \leftarrow R_3 - R_1$:

$$
\begin{pmatrix}
1 & 1 & 0 & \mid & 10 \\
0 & 1 & 1 & \mid & 8 \\
0 & -1 & -1 & \mid & -8 \\
\end{pmatrix}
$$

To eliminate the entry below the pivot in the second column, apply the row operation $R_3 \leftarrow R_3 + R_2$:

$$
\begin{pmatrix}
1 & 1 & 0 & \mid & 10 \\
0 & 1 & 1 & \mid & 8 \\
0 & 0 & 0 & \mid & 0 \\
\end{pmatrix}
$$

The matrix is now in row echelon form. Since there are $n = 3$ variables and $r = 2$ nonzero rows, there is $3 - 2 = 1$ free variable. Assigning the free parameter $x_3 = t$ ($t \in \mathbb{R}$):

From the second row ($x_2 + x_3 = 8$), we obtain:

$$
x_2 + t = 8 \implies x_2 = 8 - t
$$

Substitute $x_2 = 8 - t$ into the first row ($x_1 + x_2 = 10$):

$$
x_1 + (8 - t) = 10 \implies x_1 = 2 + t
$$

Thus, the complete solution set in parametric form is:

$$
\begin{cases}
x_1 = 2 + t, \\
x_2 = 8 - t, \\
x_3 = t,
\end{cases}
\quad (t \in \mathbb{R})
$$

### 2. Checking Equation Independence

No, all three equations are **not** independently necessary to describe the solution set. During elimination, the third row reduced completely to $(0 \quad 0 \quad 0 \mid 0)$, which shows that the third equation adds no new constraint beyond what is already imposed by the first two equations.

### 3. Deriving the Third Equation from the First Two

We can show directly by calculation that the third equation follows by subtracting the second equation from the first equation:

$$
(x_1 + x_2) - (x_2 + x_3) = 10 - 8
$$

Simplifying both sides:

$$
x_1 + x_2 - x_2 - x_3 = 2 \implies x_1 - x_3 = 2
$$

Because the third equation is an exact linear combination ($E_1 - E_2$) of the first two equations, removing it leaves the solution set completely unchanged.
