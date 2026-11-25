# Exercise 14. A System of Equations and the Determinant

Consider the system $Ax = b$, where

$$
A =
\begin{pmatrix}
1 & 2 \\
k & 4 \\
\end{pmatrix}
$$

For which values of $k$ does the system have exactly one solution for every $b$? For the remaining value, give an example of a right-hand side $b$ for which the system has infinitely many solutions, and an example for which it has no solution.

---

## Solution

**1. Condition for a Unique Solution**

A square linear system $Ax = b$ has a unique solution for every right-hand side vector $b$ if and only if the coefficient matrix $A$ is invertible, which is equivalent to $\det A \neq 0$.

Computing the determinant of $A$:

$$
\det A = 1(4) - 2(k) = 4 - 2k
$$

Setting $\det A \neq 0$:

$$
4 - 2k \neq 0 \implies 2k \neq 4 \implies k \neq 2
$$

Therefore, the system has exactly one solution for every $b$ whenever $k \neq 2$.

---

**2. Analysis of the Exceptional Case ($k = 2$)**

When $k = 2$, the coefficient matrix becomes

$$
A =
\begin{pmatrix}
1 & 2 \\
2 & 4 \\
\end{pmatrix}
$$

Let

$$
b =
\begin{pmatrix}
b_1 \\
b_2 \\
\end{pmatrix}
$$

The augmented matrix of the system is

$$
\begin{pmatrix}
1 & 2 & \mid & b_1 \\
2 & 4 & \mid & b_2 \\
\end{pmatrix}
$$

Applying the row operation $R_2 \leftarrow R_2 - 2R_1$:

$$
\begin{pmatrix}
1 & 2 & \mid & b_1 \\
0 & 0 & \mid & b_2 - 2b_1 \\
\end{pmatrix}
$$

From the second row, the consistency of the system depends on the condition $b_2 - 2b_1 = 0$, or equivalently $b_2 = 2b_1$.

- **Example for Infinitely Many Solutions:**

  Choose $b_1 = 1$ and $b_2 = 2$ so that $b_2 = 2b_1$ holds:

  $$
  b =
  \begin{pmatrix}
  1 \\
  2 \\
  \end{pmatrix}
  $$

  With this choice, the second equation reduces to $0 = 0$, leaving one free variable and infinitely many solutions.

- **Example for No Solution:**

  Choose $b_1 = 1$ and $b_2 = 3$ so that $b_2 \neq 2b_1$:

  $$
  b =
  \begin{pmatrix}
  1 \\
  3 \\
  \end{pmatrix}
  $$

  With this choice, the second equation becomes $0 = 1$, which is inconsistent and yields no solution.



