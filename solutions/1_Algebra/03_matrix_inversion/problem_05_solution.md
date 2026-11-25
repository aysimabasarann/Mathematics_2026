
# Exercise 5 – A 3×3 Matrix

## Solution

Given:

\[
A=
\begin{pmatrix}
1&1&0\\
0&1&1\\
1&0&1
\end{pmatrix}
\]

We use the Gauss–Jordan method.

### Step 1. Form the Augmented Matrix

\[
[A|I]=
\left(
\begin{array}{ccc|ccc}
1&1&0&1&0&0\\
0&1&1&0&1&0\\
1&0&1&0&0&1
\end{array}
\right)
\]

### Step 2. Eliminate the First Entry in Row 3

Apply:

\[
R_3\leftarrow R_3-R_1
\]

\[
\left(
\begin{array}{ccc|ccc}
1&1&0&1&0&0\\
0&1&1&0&1&0\\
0&-1&1&-1&0&1
\end{array}
\right)
\]

### Step 3. Make the Second Entry in Row 3 Positive

Apply:

\[
R_3\leftarrow -R_3
\]

\[
\left(
\begin{array}{ccc|ccc}
1&1&0&1&0&0\\
0&1&1&0&1&0\\
0&1&-1&1&0&-1
\end{array}
\right)
\]

### Step 4. Eliminate the Second Entry in Row 3

Apply:

\[
R_3\leftarrow R_3-R_2
\]

\[
\left(
\begin{array}{ccc|ccc}
1&1&0&1&0&0\\
0&1&1&0&1&0\\
0&0&-2&1&-1&-1
\end{array}
\right)
\]

### Step 5. Make the Third Pivot Equal to 1

Apply:

\[
R_3\leftarrow -\frac12 R_3
\]

\[
\left(
\begin{array}{ccc|ccc}
1&1&0&1&0&0\\
0&1&1&0&1&0\\
0&0&1&-\frac12&\frac12&\frac12
\end{array}
\right)
\]

### Step 6. Eliminate the Third Entry in Row 2

Apply:

\[
R_2\leftarrow R_2-R_3
\]

\[
\left(
\begin{array}{ccc|ccc}
1&1&0&1&0&0\\
0&1&0&\frac12&\frac12&-\frac12\\
0&0&1&-\frac12&\frac12&\frac12
\end{array}
\right)
\]

### Step 7. Eliminate the Second Entry in Row 1

Apply:

\[
R_1\leftarrow R_1-R_2
\]

\[
\left(
\begin{array}{ccc|ccc}
1&0&0&\frac12&-\frac12&\frac12\\
0&1&0&\frac12&\frac12&-\frac12\\
0&0&1&-\frac12&\frac12&\frac12
\end{array}
\right)
\]

### Final Result

The left side is now the identity matrix. Therefore, the right side is the inverse:

\[
\boxed{
A^{-1}=
\frac12
\begin{pmatrix}
1&-1&1\\
1&1&-1\\
-1&1&1
\end{pmatrix}
}
\]

### Verification by Multiplication

We check the result by computing \(AA^{-1}\):

\[
AA^{-1}=
\begin{pmatrix}
1&1&0\\
0&1&1\\
1&0&1
\end{pmatrix}
\frac12
\begin{pmatrix}
1&-1&1\\
1&1&-1\\
-1&1&1
\end{pmatrix}
\]

\[
=
\frac12
\begin{pmatrix}
2&0&0\\
0&2&0\\
0&0&2
\end{pmatrix}
\]

\[
=
\begin{pmatrix}
1&0&0\\
0&1&0\\
0&0&1
\end{pmatrix}
=I
\]

Therefore, the inverse is correct.

\[
\boxed{
A^{-1}=
\frac12
\begin{pmatrix}
1&-1&1\\
1&1&-1\\
-1&1&1
\end{pmatrix}
}
\]
