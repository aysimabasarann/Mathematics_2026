### Exercise 2. Determinant of a 3×3 Matrix

For

$$
A=
\begin{pmatrix}
1 & 2 & -1 \\
0 & 3 & 4 \\
2 & 1 & 5 \\
\end{pmatrix}
$$

compute $\det A$ using Sarrus' rule. Then perform one simple check using a chosen property of the determinant.

---

## Solution

### 1. Computing $\det A$ Using Sarrus' Rule

To apply Sarrus' rule, we repeat the first two columns of $A$ to the right of the matrix:

$$
\begin{pmatrix}
1 & 2 & -1 & \mid & 1 & 2 \\
0 & 3 & 4 & \mid & 0 & 3 \\
2 & 1 & 5 & \mid & 2 & 1 \\
\end{pmatrix}
$$

Next, we compute the sum of the products along the three main diagonals (top-left to bottom-right):

$$
D_1 = (1)(3)(5) + (2)(4)(2) + (-1)(0)(1) = 15 + 16 + 0 = 31
$$

Then, we compute the sum of the products along the three anti-diagonals (bottom-left to top-right):

$$
D_2 = (2)(3)(-1) + (1)(4)(1) + (5)(0)(2) = -6 + 4 + 0 = -2
$$

Subtracting $D_2$ from $D_1$ yields the determinant:

$$
\det A = D_1 - D_2 = 31 - (-2) = 33
$$

### 2. Verification Using a Determinant Property

We use the property that adding a multiple of one row to another row does not change the determinant.

Applying the row operation $R_3 \leftarrow R_3 - 2R_1$ to eliminate the bottom-left entry produces an equivalent matrix $B$ with $\det B = \det A$:

$$
B =
\begin{pmatrix}
1 & 2 & -1 \\
0 & 3 & 4 \\
0 & -3 & 7 \\
\end{pmatrix}
$$

Next, applying $R_3 \leftarrow R_3 + R_2$ yields an upper-triangular matrix $U$ with $\det U = \det A$:

$$
U =
\begin{pmatrix}
1 & 2 & -1 \\
0 & 3 & 4 \\
0 & 0 & 11 \\
\end{pmatrix}
$$

The determinant of an upper-triangular matrix is the product of its main diagonal entries:

$$
\det A = \det U = (1)(3)(11) = 33
$$

Both methods give $33$, confirming the result.

  
