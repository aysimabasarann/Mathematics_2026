
# Problem 02 – Determinant of a 3x3 Matrix

## Solution

Given:

\[
A = \begin{pmatrix}
1 & 2 & -1 \\
0 & 3 & 4 \\
2 & 1 & 5
\end{pmatrix}
\]

### 1. Calculate the determinant using Sarrus' rule

For a 3x3 matrix, Sarrus' rule gives:

\[
\det(A) =
aei+bfg+cdh-ceg-bdi-afh
\]

Substituting the matrix entries:

\[
\det(A) =
(1\cdot3\cdot5)
+(2\cdot4\cdot2)
+(-1\cdot0\cdot1)
\]

\[
-(-1\cdot3\cdot2)
-(2\cdot0\cdot5)
-(1\cdot4\cdot1)
\]

Calculate the positive diagonals:

\[
15+16+0=31
\]

Calculate the negative diagonals:

\[
-6+0+4=-2
\]

Therefore:

\[
\det(A)=31-(-2)
\]

\[
\boxed{\det(A)=33}
\]

### 2. Check using a determinant property

Adding a multiple of one row to another row does not change the determinant.

Apply the operation:

\[
R_3 \leftarrow R_3-2R_1
\]

The new matrix becomes:

\[
A' = \begin{pmatrix}
1 & 2 & -1 \\
0 & 3 & 4 \\
0 & -3 & 7
\end{pmatrix}
\]

Expanding along the first column:

\[
\det(A') =
1\begin{vmatrix}
3 & 4 \\
-3 & 7
\end{vmatrix}
\]

\[
\det(A')=1(3\cdot7-4\cdot(-3))
\]

\[
\det(A')=21+12
\]

\[
\det(A')=33
\]

Since the row operation does not change the determinant:

\[
\det(A)=\det(A')=33
\]

### Final Answer

\[
\boxed{\det(A)=33}
\]

Both calculations give the same result, so the determinant is verified.
