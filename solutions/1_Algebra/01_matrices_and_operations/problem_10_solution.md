
# Problem 10 – Columns of a Matrix Product

## Solution

Given:

\[
A = \begin{pmatrix}
1 & 2 & 0 \\
0 & 1 & 1
\end{pmatrix},
\quad
B = \begin{pmatrix}
1 & 2 \\
-1 & 0 \\
3 & 1
\end{pmatrix}
\]

The columns of B are:

\[
b_1 = \begin{pmatrix} 1 \\ -1 \\ 3 \end{pmatrix},
\quad
b_2 = \begin{pmatrix} 2 \\ 0 \\ 1 \end{pmatrix}
\]

### 1. Compute Ab₁ and Ab₂

First, calculate Ab₁.

\[
Ab_1 =
\begin{pmatrix}
1 & 2 & 0 \\
0 & 1 & 1
\end{pmatrix}
\begin{pmatrix}
1 \\ -1 \\ 3
\end{pmatrix}
\]

\[
Ab_1 =
\begin{pmatrix}
1-2+0 \\
0-1+3
\end{pmatrix}
=
\begin{pmatrix}
-1 \\ 2
\end{pmatrix}
\]

Now, calculate Ab₂.

\[
Ab_2 =
\begin{pmatrix}
1 & 2 & 0 \\
0 & 1 & 1
\end{pmatrix}
\begin{pmatrix}
2 \\ 0 \\ 1
\end{pmatrix}
\]

\[
Ab_2 =
\begin{pmatrix}
2+0+0 \\
0+0+1
\end{pmatrix}
=
\begin{pmatrix}
2 \\ 1
\end{pmatrix}
\]

### 2. Compute the matrix AB

We multiply A by B.

\[
AB =
\begin{pmatrix}
1 & 2 & 0 \\
0 & 1 & 1
\end{pmatrix}
\begin{pmatrix}
1 & 2 \\
-1 & 0 \\
3 & 1
\end{pmatrix}
\]

\[
AB =
\begin{pmatrix}
1-2+0 & 2+0+0 \\
0-1+3 & 0+0+1
\end{pmatrix}
\]

\[
AB =
\begin{pmatrix}
-1 & 2 \\
2 & 1
\end{pmatrix}
\]

### 3. Compare the results

The columns of AB are:

\[
\begin{pmatrix} -1 \\ 2 \end{pmatrix},
\quad
\begin{pmatrix} 2 \\ 1 \end{pmatrix}
\]

These are exactly the vectors Ab₁ and Ab₂.

Therefore, the first column of AB is Ab₁, and the second column is Ab₂.

### 4. Explanation

When two matrices are multiplied, each column of the resulting matrix is obtained by multiplying the first matrix by the corresponding column of the second matrix.

This is because matrix multiplication applies A to each column of B separately.

### Final Answer

\[
Ab_1 = \begin{pmatrix} -1 \\ 2 \end{pmatrix}
\]

\[
Ab_2 = \begin{pmatrix} 2 \\ 1 \end{pmatrix}
\]

\[
\boxed{
AB = \begin{pmatrix}
-1 & 2 \\
2 & 1
\end{pmatrix}
}
\]

The columns of AB are exactly Ab₁ and Ab₂.
