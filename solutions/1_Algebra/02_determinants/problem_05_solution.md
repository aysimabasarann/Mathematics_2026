### Exercise 5. Row Operations

For

$$
A=
\begin{pmatrix}
1 & 2 & 3 \\
2 & 1 & 0 \\
-1 & 4 & 2 \\
\end{pmatrix}
$$

find $\det A$ by simplifying the matrix with row operations. At each step, indicate whether and how the determinant changes.

---

## Solution

### 1. Applying Row Operations to Simplify the Matrix

We use elementary row operations to transform matrix $A$ into an upper-triangular form while tracking how each operation affects the determinant.

**Step 1:** Eliminate the entry below the leading entry in the first column by applying $R_2 \leftarrow R_2 - 2R_1$ and $R_3 \leftarrow R_3 + R_1$.
* Adding a multiple of one row to another row **does not change the value of the determinant**.

$$
A_1 =
\begin{pmatrix}
1 & 2 & 3 \\
0 & -3 & -6 \\
0 & 6 & 5 \\
\end{pmatrix}
$$

**Step 2:** Eliminate the entry below the leading entry in the second column by applying $R_3 \leftarrow R_3 + 2R_2$.
* Adding a multiple of one row to another row **still does not change the determinant**.

$$
A_2 =
\begin{pmatrix}
1 & 2 & 3 \\
0 & -3 & -6 \\
0 & 0 & -7 \\
\end{pmatrix}
$$

### 2. Computing the Determinant

Now that the matrix is in upper-triangular form, its determinant is simply the product of its main diagonal entries:

$$
\det A = (1)(-3)(-7) = 21
$$

Since all applied operations were row additions/replacements (which preserve the determinant), the determinant of the original matrix $A$ is $21$.

 
