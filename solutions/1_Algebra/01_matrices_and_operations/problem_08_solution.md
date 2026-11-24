
# Problem 08 – Row Operations and Their Reversibility

## Solution

Given:

\[
A = \begin{pmatrix}
1 & 2 & -1 \\
2 & 4 & 1 \\
-1 & 1 & 3
\end{pmatrix}
\]

### 1. First operation: R₂ ← R₂ − 2R₁

We subtract twice the first row from the second row.

\[
R_2 = (2,4,1)-2(1,2,-1)
\]

\[
R_2 = (2,4,1)-(2,4,-2)
\]

\[
R_2 = (0,0,3)
\]

The resulting matrix is:

\[
A_1 = \begin{pmatrix}
1 & 2 & -1 \\
0 & 0 & 3 \\
-1 & 1 & 3
\end{pmatrix}
\]

The reverse operation is:

\[
R_2 \leftarrow R_2 + 2R_1
\]

### 2. Second operation: R₃ ← R₃ + R₁

We add the first row to the third row.

\[
R_3 = (-1,1,3)+(1,2,-1)
\]

\[
R_3 = (0,3,2)
\]

The resulting matrix is:

\[
A_2 = \begin{pmatrix}
1 & 2 & -1 \\
0 & 0 & 3 \\
0 & 3 & 2
\end{pmatrix}
\]

The reverse operation is:

\[
R_3 \leftarrow R_3 - R_1
\]

### 3. Third operation: Interchange R₂ and R₃

We exchange the second and third rows.

The resulting matrix is:

\[
A_3 = \begin{pmatrix}
1 & 2 & -1 \\
0 & 3 & 2 \\
0 & 0 & 3
\end{pmatrix}
\]

The reverse operation is also:

\[
R_2 \leftrightarrow R_3
\]

### 4. Explanation

Each elementary row operation is reversible.

- Adding or subtracting a multiple of one row can be reversed by performing the opposite operation.
- Interchanging two rows can be reversed by interchanging them again.

Therefore, all three row operations have inverse operations.

### Final Answer

The final matrix is:

\[
\boxed{
\begin{pmatrix}
1 & 2 & -1 \\
0 & 3 & 2 \\
0 & 0 & 3
\end{pmatrix}
}
\]

The reverse operations are:

1. \(R_2 \leftarrow R_2 + 2R_1\)
2. \(R_3 \leftarrow R_3 - R_1\)
3. \(R_2 \leftrightarrow R_3\)
