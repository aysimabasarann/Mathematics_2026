### Exercise 3. When Does the Inverse Not Exist?

For

$$
A=
\begin{pmatrix}
2 & 4 \\
1 & 2 \\
\end{pmatrix}
$$

explain in two ways why $A^{-1}$ does not exist: using the determinant and using dependence between the rows.

---

## Solution

### 1. Explanation Using the Determinant

For a $2 \times 2$ matrix $A = \begin{pmatrix} a & b \\ c & d \end{pmatrix}$, the inverse formula requires dividing by its determinant:

$$
\det A = ad - bc
$$

For the given matrix $A$, we compute the determinant:

$$
\det A = (2)(2) - (4)(1) = 4 - 4 = 0
$$

Since the determinant is zero ($\det A = 0$), the formula for the inverse involves division by zero, which is undefined. Therefore, the inverse matrix $A^{-1}$ does not exist.

### 2. Explanation Using Row Dependence

Let $R_1$ and $R_2$ denote the rows of matrix $A$:

$$
R_1 = (2, 4), \qquad R_2 = (1, 2)
$$

Observing the components, the first row is a scalar multiple of the second row:

$$
R_1 = 2R_2
$$

This indicates that the rows of $A$ are linearly dependent. A fundamental property of square matrices states that a matrix is invertible if and only if its rows (and columns) are linearly independent. Because the rows are dependent, the matrix collapses dimensions and is thus noninvertible.



