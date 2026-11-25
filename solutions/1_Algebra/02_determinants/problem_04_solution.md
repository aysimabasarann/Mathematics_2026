### Exercise 4. Triangular Matrix

Without expanding the determinant, compute

$$
\det
\begin{pmatrix}
2 & 4 & 1 \\
0 & -3 & 5 \\
0 & 0 & 7 \\
\end{pmatrix}.
$$

State the rule for an arbitrary triangular matrix and explain it using this example.

---

## Solution

### 1. Computing the Determinant

Without performing a full expansion or using Sarrus' rule, we can recognize that the given matrix is an upper-triangular matrix, since all entries below the main diagonal are equal to zero. 

The determinant of a triangular matrix is simply the product of its main diagonal entries:

$$
\det
\begin{pmatrix}
2 & 4 & 1 \\
0 & -3 & 5 \\
0 & 0 & 7 \\
\end{pmatrix}
= (2)(-3)(7) = -42
$$

### 2. General Rule and Explanation

**General Rule:**
For any square triangular matrix (whether upper-triangular, lower-triangular, or diagonal), the determinant is equal to the product of the entries along its main diagonal:

$$
\det A = a_{11}a_{22}\cdots a_{nn}
$$

**Explanation Using This Example:**
If we compute the determinant by expanding successively along the columns containing zeros (starting with the first column):
1. Expanding along the first column leaves the top-left entry $(2)$ multiplied by the determinant of the remaining $2 \times 2$ lower-right submatrix.
2. That $2 \times 2$ submatrix is also triangular, so its expansion leaves its top-left entry $(-3)$ multiplied by the bottom-right diagonal entry $(7)$.

Thus, all off-diagonal terms vanish during the expansion process, leaving only the product of the diagonal elements.

