
# Problem 07 – Identity Matrix, Zero Matrix, and Powers

## Solution

Given:

\[
A = \begin{pmatrix} 2 & 1 \\ 0 & 2 \end{pmatrix}
\]

### 1. Calculate AI

The identity matrix is:

\[
I = \begin{pmatrix} 1 & 0 \\ 0 & 1 \end{pmatrix}
\]

Multiplying a matrix by the identity matrix does not change it.

\[
AI =
\begin{pmatrix} 2 & 1 \\ 0 & 2 \end{pmatrix}
\begin{pmatrix} 1 & 0 \\ 0 & 1 \end{pmatrix}
\]

\[
AI = \begin{pmatrix} 2 & 1 \\ 0 & 2 \end{pmatrix}
\]

### 2. Calculate IA

\[
IA =
\begin{pmatrix} 1 & 0 \\ 0 & 1 \end{pmatrix}
\begin{pmatrix} 2 & 1 \\ 0 & 2 \end{pmatrix}
\]

\[
IA = \begin{pmatrix} 2 & 1 \\ 0 & 2 \end{pmatrix}
\]

### 3. Calculate A + 0

The zero matrix is:

\[
0 = \begin{pmatrix} 0 & 0 \\ 0 & 0 \end{pmatrix}
\]

Adding the zero matrix does not change the original matrix.

\[
A+0 =
\begin{pmatrix} 2 & 1 \\ 0 & 2 \end{pmatrix}
+
\begin{pmatrix} 0 & 0 \\ 0 & 0 \end{pmatrix}
\]

\[
A+0 = \begin{pmatrix} 2 & 1 \\ 0 & 2 \end{pmatrix}
\]

### 4. Calculate A²

\[
A^2 = A \cdot A
\]

\[
A^2 =
\begin{pmatrix} 2 & 1 \\ 0 & 2 \end{pmatrix}
\begin{pmatrix} 2 & 1 \\ 0 & 2 \end{pmatrix}
\]

\[
A^2 =
\begin{pmatrix}
2\cdot2+1\cdot0 & 2\cdot1+1\cdot2 \\
0\cdot2+2\cdot0 & 0\cdot1+2\cdot2
\end{pmatrix}
\]

\[
A^2 = \begin{pmatrix} 4 & 4 \\ 0 & 4 \end{pmatrix}
\]

### 5. Calculate A³

\[
A^3 = A^2 \cdot A
\]

\[
A^3 =
\begin{pmatrix} 4 & 4 \\ 0 & 4 \end{pmatrix}
\begin{pmatrix} 2 & 1 \\ 0 & 2 \end{pmatrix}
\]

\[
A^3 =
\begin{pmatrix}
4\cdot2+4\cdot0 & 4\cdot1+4\cdot2 \\
0\cdot2+4\cdot0 & 0\cdot1+4\cdot2
\end{pmatrix}
\]

\[
A^3 = \begin{pmatrix} 8 & 12 \\ 0 & 8 \end{pmatrix}
\]

### 6. Explanation

The identity matrix I does not change a matrix when multiplied by it.

The zero matrix 0 does not change a matrix when added to it.

The successive powers of A show a pattern:

\[
A^1 = \begin{pmatrix} 2 & 1 \\ 0 & 2 \end{pmatrix}
\]

\[
A^2 = \begin{pmatrix} 4 & 4 \\ 0 & 4 \end{pmatrix}
\]

\[
A^3 = \begin{pmatrix} 8 & 12 \\ 0 & 8 \end{pmatrix}
\]

The diagonal entries double in each successive power, while the upper-right entry follows the sequence 1, 4, 12.

### Final Answer

\[
AI = IA = A
\]

\[
A+0 = A
\]

\[
A^2 = \begin{pmatrix} 4 & 4 \\ 0 & 4 \end{pmatrix}
\]

\[
A^3 = \begin{pmatrix} 8 & 12 \\ 0 & 8 \end{pmatrix}
\]

The identity matrix is the neutral element of matrix multiplication, and the zero matrix is the neutral element of matrix addition.
