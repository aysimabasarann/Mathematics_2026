### Exercise 11. Shortening the Calculation with Row Operations

Compute

$$
\det
\begin{pmatrix}
1 & 2 & 3 \\
1 & 3 & 4 \\
1 & 4 & 6 \\
\end{pmatrix}
$$

by first performing row operations that create as many zeros as possible. State which operations do not change the determinant.

---

## Solution

### 1. Creating Zeros via Determinant-Preserving Row Operations

We apply elementary row operations to transform the matrix into upper-triangular form.

**Step 1:** Eliminate the entries below the leading $1$ in the first column by performing:

$$
R_2 \leftarrow R_2 - R_1, \qquad R_3 \leftarrow R_3 - R_1
$$

This produces:

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 1 \\
0 & 2 & 3 \\
\end{pmatrix}
$$

**Step 2:** Eliminate the entry below the leading $1$ in the second column by performing:

$$
R_3 \leftarrow R_3 - 2R_2
$$

This produces an upper-triangular matrix:

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 1 \\
0 & 0 & 1 \\
\end{pmatrix}
$$

### 2. Computing the Determinant

The determinant of an upper-triangular matrix is the product of its main diagonal entries:

$$
\det
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 1 \\
0 & 0 & 1 \\
\end{pmatrix}
= (1)(1)(1) = 1
$$

### 3. Effect of the Operations on the Determinant

**Property:** Adding a scalar multiple of one row to another row ($R_i \leftarrow R_i + kR_j$) **does not change the value of the determinant**. Because all three operations used ($R_2 \leftarrow R_2 - R_1$, $R_3 \leftarrow R_3 - R_1$, and $R_3 \leftarrow R_3 - 2R_2$) are row-addition operations of this type, the determinant remains unchanged at every step, giving:

$$
\det
\begin{pmatrix}
1 & 2 & 3 \\
1 & 3 & 4 \\
1 & 4 & 6 \\
\end{pmatrix}
= 1
$$

 

