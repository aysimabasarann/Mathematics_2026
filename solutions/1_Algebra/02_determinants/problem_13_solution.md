
# Exercise 13 – Determinant by Elimination

## Solution

Given:

\[
A=
\begin{pmatrix}
1&2&3\\
2&5&7\\
1&0&2
\end{pmatrix}
\]

### Step 1. Eliminate the first column

First, perform:

\[
R_2\leftarrow R_2-2R_1
\]

Then:

\[
R_3\leftarrow R_3-R_1
\]

The matrix becomes:

\[
\begin{pmatrix}
1&2&3\\
0&1&1\\
0&-2&-1
\end{pmatrix}
\]

These operations do not change the determinant.

### Step 2. Eliminate the second column

Perform:

\[
R_3\leftarrow R_3+2R_2
\]

We obtain:

\[
\begin{pmatrix}
1&2&3\\
0&1&1\\
0&0&1
\end{pmatrix}
\]

This operation also does not change the determinant.

### Step 3. Calculate the determinant

The resulting matrix is upper triangular.

Therefore, its determinant is the product of its diagonal entries:

\[
\det(A)=1\cdot1\cdot1
\]

\[
\boxed{\det(A)=1}
\]

### Step 4. Explain the effect of row operations

All operations used were of the form:

\[
R_i\leftarrow R_i+kR_j
\]

These operations do not change the determinant.

No rows were exchanged and no row was multiplied by a scalar.

### Final Answer

\[
\boxed{\det(A)=1}
\]

The determinant remains unchanged throughout the elimination process because adding a multiple of one row to another row does not affect the determinant.
