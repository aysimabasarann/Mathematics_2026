
# Problem 05 – Matrix Times Vector

## Solution

Given:

\[
A = \begin{pmatrix} 2 & -1 \\ 1 & 3 \end{pmatrix},
\quad
x = \begin{pmatrix} 4 \\ 2 \end{pmatrix}
\]

### 1. Calculate Ax

We multiply each row of matrix A by the vector x.

\[
Ax =
\begin{pmatrix}
2\cdot4+(-1)\cdot2 \\
1\cdot4+3\cdot2
\end{pmatrix}
\]

\[
Ax =
\begin{pmatrix}
8-2 \\
4+6
\end{pmatrix}
=
\begin{pmatrix}
6 \\
10
\end{pmatrix}
\]

### 2. Express Ax as a linear combination

The columns of matrix A are:

\[
a_1 = \begin{pmatrix} 2 \\ 1 \end{pmatrix},
\quad
a_2 = \begin{pmatrix} -1 \\ 3 \end{pmatrix}
\]

The vector x contains the coefficients 4 and 2.

Therefore:

\[
Ax = 4a_1 + 2a_2
\]

Substituting the column vectors:

\[
Ax =
4\begin{pmatrix} 2 \\ 1 \end{pmatrix}
+
2\begin{pmatrix} -1 \\ 3 \end{pmatrix}
\]

\[
Ax =
\begin{pmatrix} 8 \\ 4 \end{pmatrix}
+
\begin{pmatrix} -2 \\ 6 \end{pmatrix}
\]

\[
Ax = \begin{pmatrix} 6 \\ 10 \end{pmatrix}
\]

### Final Answer

\[
\boxed{Ax = \begin{pmatrix} 6 \\ 10 \end{pmatrix}}
\]

The matrix-vector product is a linear combination of the columns of A, using the entries of x as coefficients.
