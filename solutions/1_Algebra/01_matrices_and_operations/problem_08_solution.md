### Exercise 8. Row Operations and Their Reversibility

**Problem:**

For

$$
A = \begin{pmatrix}
1 & 2 & -1 \\
2 & 4 & 1 \\
-1 & 1 & 3
\end{pmatrix}
$$

perform, in order:

1. $R_2 \leftarrow R_2 - 2R_1$,
2. $R_3 \leftarrow R_3 + R_1$,
3. interchange $R_2$ and $R_3$.

Write the matrix after each step. Then, for each of the three operations, state an operation that reverses it.

---

## Solution

### 1. Initial Matrix

The starting matrix is:

$$
A_0 = \begin{pmatrix}
1 & 2 & -1 \\
2 & 4 & 1 \\
-1 & 1 & 3
\end{pmatrix}
$$

### 2. Step 1: $R_2 \leftarrow R_2 - 2R_1$

We subtract $2$ times the first row from the second row:

$$
A_1 = \begin{pmatrix}
1 & 2 & -1 \\
2 - 2(1) & 4 - 2(2) & 1 - 2(-1) \\
-1 & 1 & 3
\end{pmatrix}
= \begin{pmatrix}
1 & 2 & -1 \\
0 & 0 & 3 \\
-1 & 1 & 3
\end{pmatrix}
$$

* **Reversing Operation:** To undo $R_2 \leftarrow R_2 - 2R_1$, we add $2$ times the first row to the second row ($R_2 \leftarrow R_2 + 2R_1$).

### 3. Step 2: $R_3 \leftarrow R_3 + R_1$

We add the first row to the third row of the matrix obtained in Step 1:

$$
A_2 = \begin{pmatrix}
1 & 2 & -1 \\
0 & 0 & 3 \\
-1 + 1 & 1 + 2 & 3 + (-1)
\end{pmatrix}
= \begin{pmatrix}
1 & 2 & -1 \\
0 & 0 & 3 \\
0 & 3 & 2
\end{pmatrix}
$$

* **Reversing Operation:** To undo $R_3 \leftarrow R_3 + R_1$, we subtract the first row from the third row ($R_3 \leftarrow R_3 - R_1$).

### 4. Step 3: Interchange $R_2$ and $R_3$

We swap the second and third rows of the matrix obtained in Step 2:

$$
A_3 = \begin{pmatrix}
1 & 2 & -1 \\
0 & 3 & 2 \\
0 & 0 & 3
\end{pmatrix}
$$

* **Reversing Operation:** To undo the interchange of $R_2$ and $R_3$, we simply interchange $R_2$ and $R_3$ again.

