
# Exercise 12 – A Parameter Revealed by a Row Operation

## Solution

Given:

\[
A(t)=
\begin{pmatrix}
1&2&3\\
2&4&t\\
0&1&1
\end{pmatrix}
\]

### Step 1. Perform the given row operation

\[
R_2\leftarrow R_2-2R_1
\]

We obtain:

\[
\begin{pmatrix}
1&2&3\\
0&0&t-6\\
0&1&1
\end{pmatrix}
\]

This row operation does not change the determinant.

### Step 2. Calculate the determinant

Expanding along the first column:

\[
\det A(t)=
\begin{vmatrix}
0&t-6\\
1&1
\end{vmatrix}
\]

\[
=0\cdot1-(t-6)\cdot1
\]

\[
\det A(t)=6-t
\]

### Step 3. Find the values for which the matrix is not invertible

A matrix is not invertible when its determinant is zero.

\[
6-t=0
\]

Therefore:

\[
\boxed{t=6}
\]

### Step 4. Explain the special relationship between the rows

When \(t=6\), the matrix becomes:

\[
A(6)=
\begin{pmatrix}
1&2&3\\
2&4&6\\
0&1&1
\end{pmatrix}
\]

Notice that the second row is exactly twice the first row:

\[
R_2=2R_1
\]

After the row operation, the second row becomes a zero row.

This means that the rows are linearly dependent, so the determinant is zero and the matrix is not invertible.

### Final Answer

\[
\boxed{t=6}
\]

The matrix is not invertible when \(t=6\), because its second row becomes twice its first row, creating linear dependence.
