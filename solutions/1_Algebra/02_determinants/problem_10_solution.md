### Exercise 10. Detecting Dependence

Without carrying out a full determinant calculation, explain why

$$
\det
\begin{pmatrix}
1 & 2 & 3 \\
2 & 4 & 6 \\
0 & 1 & 5 \\
\end{pmatrix}
= 0.
$$

Identify a specific dependence between the rows and connect it with noninvertibility of the matrix.

---

## Solution

### 1. Identifying the Row Dependence

Let $R_1$, $R_2$, and $R_3$ denote the first, second, and third rows of the matrix, respectively:

$$
R_1 =
\begin{pmatrix}
1 & 2 & 3 \\
\end{pmatrix},\qquad
R_2 =
\begin{pmatrix}
2 & 4 & 6 \\
\end{pmatrix},\qquad
R_3 =
\begin{pmatrix}
0 & 1 & 5 \\
\end{pmatrix}
$$

Comparing $R_1$ and $R_2$, every entry in the second row is exactly twice the corresponding entry in the first row:

$$
R_2 = 2R_1
$$

Thus, the rows of the matrix are linearly dependent (specifically, one row is a scalar multiple of another).

### 2. Why the Determinant Is Zero

A fundamental property of determinants states that if one row of a square matrix is a scalar multiple of another row, the determinant of the matrix is zero. 

Alternatively, applying the determinant-preserving row operation $R_2 \leftarrow R_2 - 2R_1$ produces a matrix with an entire row of zeros:

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & 0 & 0 \\
0 & 1 & 5 \\
\end{pmatrix}
$$

Since any matrix containing a zero row has a determinant of $0$, it follows immediately that $\det A = 0$ without needing any expansion.

### 3. Connection with Noninvertibility

A square matrix is invertible if and only if its rows (and columns) are linearly independent, which is equivalent to having a non-zero determinant. Because the linear dependence $R_2 = 2R_1$ causes the rows to span a subspace of dimension strictly less than $3$ (collapsing the $3$-dimensional volume to zero), the matrix cannot be reversed by any inverse transformation and is therefore **not invertible**.

