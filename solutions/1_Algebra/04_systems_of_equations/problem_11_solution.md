### Exercise 11. A Parameter in a System of Three Equations

Analyze the number of solutions depending on $t$:

$$
\begin{cases}
x+y+z=1, \\
x+ty+z=2, \\
x+y+tz=3.
\end{cases}
$$

Use elimination and separately analyze the parameter values for which a standard calculation step ceases to be valid.

---

## Solution

### 1. Elimination on the Augmented Matrix

We write the system as an augmented matrix:

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 1 \\
1 & t & 1 & \mid & 2 \\
1 & 1 & t & \mid & 3 \\
\end{pmatrix}
$$

To eliminate the entries below the first pivot in column 1, apply the row operations $R_2 \leftarrow R_2 - R_1$ and $R_3 \leftarrow R_3 - R_1$:

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 1 \\
0 & t - 1 & 0 & \mid & 1 \\
0 & 0 & t - 1 & \mid & 2 \\
\end{pmatrix}
$$

The matrix is now in upper triangular form, corresponding to the system:

$$
\begin{cases}
x + y + z = 1, \\
(t - 1)y = 1, \\
(t - 1)z = 2.
\end{cases}
$$

### 2. Identifying Critical Parameter Values

In standard back-substitution, we would divide the second and third equations by $(t - 1)$ to solve for $y$ and $z$. This division ceases to be valid when the divisor equals zero:

$$
t - 1 = 0 \implies t = 1
$$

Therefore, $t = 1$ is the unique critical parameter value that must be analyzed separately.

### 3. Case-by-Case Analysis

- **Case 1: When $t = 1$**

  Substituting $t = 1$ into the reduced augmented matrix gives:

  $$
  \begin{pmatrix}
  1 & 1 & 1 & \mid & 1 \\
  0 & 0 & 0 & \mid & 1 \\
  0 & 0 & 0 & \mid & 2 \\
  \end{pmatrix}
  $$

  The second and third rows correspond to the equations $0 = 1$ and $0 = 2$, both of which are contradictions. Therefore, for $t = 1$, the system is inconsistent and has **no solution**.

- **Case 2: When $t \neq 1$**

  Since $t - 1 \neq 0$, we can safely divide the second and third equations by $t - 1$:

  $$
  y = \frac{1}{t - 1}, \qquad z = \frac{2}{t - 1}
  $$

  Substitute these expressions for $y$ and $z$ back into the first equation $x + y + z = 1$:

  $$
  x + \frac{1}{t - 1} + \frac{2}{t - 1} = 1
  $$

  Combine the fractions and solve for $x$:

  $$
  x + \frac{3}{t - 1} = 1 \implies x = 1 - \frac{3}{t - 1} = \frac{(t - 1) - 3}{t - 1} = \frac{t - 4}{t - 1}
  $$

  Because every variable is uniquely determined in terms of $t$, the system has **exactly one solution** for all $t \neq 1$, given by:

  $$
  (x, y, z) = \left(\frac{t - 4}{t - 1}, \frac{1}{t - 1}, \frac{2}{t - 1}\right)
  $$

### 4. Summary of Results

- **No solution:** occurs when $t = 1$.
- **Infinitely many solutions:** never occurs for any value of $t$.
- **Exactly one solution:** occurs for all $t \neq 1$.
