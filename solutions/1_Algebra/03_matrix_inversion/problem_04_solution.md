
# Exercise 4 – Gauss–Jordan Method

## Solution

Given:

\[
A=
\begin{pmatrix}
1&2\\
3&5
\end{pmatrix}
\]

To find the inverse, start with the augmented matrix:

\[
[A|I]=
\left(
\begin{array}{cc|cc}
1&2&1&0\\
3&5&0&1
\end{array}
\right)
\]

### Step 1. Eliminate the First Entry in Row 2

Apply the row operation:

\[
R_2\leftarrow R_2-3R_1
\]

\[
\left(
\begin{array}{cc|cc}
1&2&1&0\\
0&-1&-3&1
\end{array}
\right)
\]

### Step 2. Make the Pivot Equal to 1

Apply:

\[
R_2\leftarrow -R_2
\]

\[
\left(
\begin{array}{cc|cc}
1&2&1&0\\
0&1&3&-1
\end{array}
\right)
\]

### Step 3. Eliminate the Second Entry in Row 1

Apply:

\[
R_1\leftarrow R_1-2R_2
\]

\[
\left(
\begin{array}{cc|cc}
1&0&-5&2\\
0&1&3&-1
\end{array}
\right)
\]

### Final Result

The left side is now the identity matrix. Therefore, the right side is the inverse:

\[
\boxed{
A^{-1}=
\begin{pmatrix}
-5&2\\
3&-1
\end{pmatrix}
}
\]

### Why Does This Method Work?

Each elementary row operation is equivalent to multiplying the matrix on the left by an elementary matrix.

When the left side becomes the identity matrix, the same operations have transformed the identity matrix into the inverse of A.

Therefore:

\[
[A|I]\longrightarrow[I|A^{-1}]
\]

This is the Gauss–Jordan method.
