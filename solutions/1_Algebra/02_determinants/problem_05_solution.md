
# Problem 05 – Row Operations

## Solution

Given:

\[
A = \begin{pmatrix}
1 & 2 & 3 \\
2 & 1 & 0 \\
-1 & 4 & 2
\end{pmatrix}
\]

### 1. Simplify the matrix using row operations

First, we eliminate the first entry of the second row.

Apply:

\[
R_2 \leftarrow R_2-2R_1
\]

The new matrix is:

\[
\begin{pmatrix}
1 & 2 & 3 \\
0 & -3 & -6 \\
-1 & 4 & 2
\end{pmatrix}
\]

This operation does not change the determinant because adding a multiple of one row to another row leaves the determinant unchanged.

### 2. Eliminate the first entry of the third row

Apply:

\[
R_3 \leftarrow R_3+R_1
\]

The matrix becomes:

\[
\begin{pmatrix}
1 & 2 & 3 \\
0 & -3 & -6 \\
0 & 6 & 5
\end{pmatrix}
\]

This operation also does not change the determinant.

### 3. Eliminate the second entry of the third row

Apply:

\[
R_3 \leftarrow R_3+2R_2
\]

The resulting matrix is:

\[
\begin{pmatrix}
1 & 2 & 3 \\
0 & -3 & -6 \\
0 & 0 & -7
\end{pmatrix}
\]

Again, the determinant remains unchanged.

### 4. Calculate the determinant

The resulting matrix is an upper triangular matrix.

The determinant of a triangular matrix is the product of its diagonal entries.

Therefore:

\[
\det(A)=1\cdot(-3)\cdot(-7)
\]

\[
\det(A)=21
\]

\[
\boxed{\det(A)=21}
\]

### 5. Explanation of determinant properties

During the solution, we used three row operations.

Each operation involved adding a multiple of one row to another row.

This type of row operation does not change the determinant.

Therefore, the determinant of the original matrix is equal to the determinant of the final triangular matrix.

### Final Answer

\[
\boxed{\det(A)=21}
\]

The determinant remains unchanged throughout all three row operations.
