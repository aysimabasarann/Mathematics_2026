### Exercise 13. Determinant by Elimination

Compute the determinant

$$
A=
\begin{pmatrix}
1 & 2 & 3 \\
2 & 5 & 7 \\
1 & 0 & 2 \\
\end{pmatrix}
$$

using elimination. Record the effect of every row operation used on the value of the determinant.

---

## Solution

### 1. Eliminating Entries Below the Main Diagonal

We use elementary row operations to reduce matrix $A$ to upper-triangular form while tracking the effect of each operation on $\det A$.

**Step 1:** Eliminate the entries below the pivot $1$ in the first column by applying:

$$
R_2 \leftarrow R_2 - 2R_1, \qquad R_3 \leftarrow R_3 - R_1
$$

* **Effect on determinant:** Adding a multiple of one row to another **does not change the value of the determinant**.

$$
A_1 =
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 1 \\
0 & -2 & -1 \\
\end{pmatrix}
$$

**Step 2:** Eliminate the entry below the pivot $1$ in the second column by applying:

$$
R_3 \leftarrow R_3 + 2R_2
$$

* **Effect on determinant:** Adding a multiple of one row to another **again leaves the determinant unchanged**.

$$
A_2 =
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 1 \\
0 & 0 & 1 \\
\end{pmatrix}
$$

### 2. Computing the Determinant

Since $A_2$ is upper-triangular, its determinant is the product of its main diagonal entries:

$$
\det A_2 = (1)(1)(1) = 1
$$

Because none of the row operations altered the value of the determinant ($\det A = \det A_1 = \det A_2$), we conclude that:

$$
\det A = 1
$$

