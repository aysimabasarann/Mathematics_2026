
# Exercise 11 – Shortening the Calculation with Row Operations

## Solution

Given:

\[
A=
\begin{pmatrix}
1&2&3\\
1&3&4\\
1&4&6
\end{pmatrix}
\]

### Step 1. Perform row operations

First, subtract the first row from the second row:

\[
R_2\leftarrow R_2-R_1
\]

Then subtract the first row from the third row:

\[
R_3\leftarrow R_3-R_1
\]

We obtain:

\[
\begin{pmatrix}
1&2&3\\
0&1&1\\
0&2&3
\end{pmatrix}
\]

### Step 2. Create another zero

Subtract twice the second row from the third row:

\[
R_3\leftarrow R_3-2R_2
\]

The matrix becomes:

\[
\begin{pmatrix}
1&2&3\\
0&1&1\\
0&0&1
\end{pmatrix}
\]

### Step 3. Calculate the determinant

The resulting matrix is upper triangular.

The determinant of a triangular matrix is the product of its diagonal entries.

\[
\det(A)=1\cdot1\cdot1
\]

\[
\boxed{\det(A)=1}
\]

### Step 4. Explain the determinant properties

All operations used were of the form:

\[
R_i\leftarrow R_i+kR_j
\]

These operations do not change the determinant.

The three elementary row operations have the following effects:

1. Swapping two rows changes the sign of the determinant.
2. Multiplying a row by a nonzero number multiplies the determinant by that number.
3. Adding a multiple of one row to another row does not change the determinant.

### Final Answer

\[
\boxed{\det(A)=1}
\]

The determinant remains unchanged because we only added multiples of one row to another row.
