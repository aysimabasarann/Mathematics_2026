
# Problem 06 – Transpose

## Solution

Given:

\[
A = \begin{pmatrix}
1 & 2 & 3 \\
4 & 5 & 6
\end{pmatrix},
\quad
B = \begin{pmatrix}
1 & 0 \\
2 & 1 \\
-1 & 3
\end{pmatrix}
\]

### 1. Calculate A^T

To find the transpose, we change the rows into columns.

\[
A^T =
\begin{pmatrix}
1 & 4 \\
2 & 5 \\
3 & 6
\end{pmatrix}
\]

### 2. Calculate B^T

Similarly, we change the rows of B into columns.

\[
B^T =
\begin{pmatrix}
1 & 2 & -1 \\
0 & 1 & 3
\end{pmatrix}
\]

### 3. Calculate AB

We multiply A by B.

\[
AB =
\begin{pmatrix}
1 & 2 & 3 \\
4 & 5 & 6
\end{pmatrix}
\begin{pmatrix}
1 & 0 \\
2 & 1 \\
-1 & 3
\end{pmatrix}
\]

\[
AB =
\begin{pmatrix}
1+4-3 & 0+2+9 \\
4+10-6 & 0+5+18
\end{pmatrix}
\]

\[
AB =
\begin{pmatrix}
2 & 11 \\
8 & 23
\end{pmatrix}
\]

### 4. Verify the transpose property

First, calculate the transpose of AB.

\[
(AB)^T =
\begin{pmatrix}
2 & 8 \\
11 & 23
\end{pmatrix}
\]

Now calculate B^T A^T.

\[
B^T A^T =
\begin{pmatrix}
1 & 2 & -1 \\
0 & 1 & 3
\end{pmatrix}
\begin{pmatrix}
1 & 4 \\
2 & 5 \\
3 & 6
\end{pmatrix}
\]

\[
B^T A^T =
\begin{pmatrix}
1+4-3 & 4+10-6 \\
0+2+9 & 0+5+18
\end{pmatrix}
\]

\[
B^T A^T =
\begin{pmatrix}
2 & 8 \\
11 & 23
\end{pmatrix}
\]

Therefore,

\[
(AB)^T = B^T A^T
\]

### Final Answer

\[
A^T =
\begin{pmatrix}
1 & 4 \\
2 & 5 \\
3 & 6
\end{pmatrix}
\]

\[
B^T =
\begin{pmatrix}
1 & 2 & -1 \\
0 & 1 & 3
\end{pmatrix}
\]

\[
AB =
\begin{pmatrix}
2 & 11 \\
8 & 23
\end{pmatrix}
\]

The identity is verified:

\[
\boxed{(AB)^T = B^T A^T}
\]
