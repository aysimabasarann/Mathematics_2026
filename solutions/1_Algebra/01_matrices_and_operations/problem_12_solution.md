
# Problem 12 – Formula for a Matrix Power

## Solution

Given:

\[
A = \begin{pmatrix} 1 & 1 \\ 0 & 1 \end{pmatrix}
\]

### 1. Calculate A²

\[
A^2 = A \cdot A
\]

\[
A^2 =
\begin{pmatrix} 1 & 1 \\ 0 & 1 \end{pmatrix}
\begin{pmatrix} 1 & 1 \\ 0 & 1 \end{pmatrix}
\]

\[
A^2 =
\begin{pmatrix}
1\cdot1+1\cdot0 & 1\cdot1+1\cdot1 \\
0\cdot1+1\cdot0 & 0\cdot1+1\cdot1
\end{pmatrix}
\]

\[
A^2 = \begin{pmatrix} 1 & 2 \\ 0 & 1 \end{pmatrix}
\]

### 2. Calculate A³

\[
A^3 = A^2 \cdot A
\]

\[
A^3 =
\begin{pmatrix} 1 & 2 \\ 0 & 1 \end{pmatrix}
\begin{pmatrix} 1 & 1 \\ 0 & 1 \end{pmatrix}
\]

\[
A^3 =
\begin{pmatrix}
1\cdot1+2\cdot0 & 1\cdot1+2\cdot1 \\
0\cdot1+1\cdot0 & 0\cdot1+1\cdot1
\end{pmatrix}
\]

\[
A^3 = \begin{pmatrix} 1 & 3 \\ 0 & 1 \end{pmatrix}
\]

### 3. Calculate A⁴

\[
A^4 = A^3 \cdot A
\]

\[
A^4 =
\begin{pmatrix} 1 & 3 \\ 0 & 1 \end{pmatrix}
\begin{pmatrix} 1 & 1 \\ 0 & 1 \end{pmatrix}
\]

\[
A^4 =
\begin{pmatrix}
1\cdot1+3\cdot0 & 1\cdot1+3\cdot1 \\
0\cdot1+1\cdot0 & 0\cdot1+1\cdot1
\end{pmatrix}
\]

\[
A^4 = \begin{pmatrix} 1 & 4 \\ 0 & 1 \end{pmatrix}
\]

### 4. Find a formula for Aⁿ

From the calculations, we observe the following pattern:

\[
A^2 = \begin{pmatrix} 1 & 2 \\ 0 & 1 \end{pmatrix}
\]

\[
A^3 = \begin{pmatrix} 1 & 3 \\ 0 & 1 \end{pmatrix}
\]

\[
A^4 = \begin{pmatrix} 1 & 4 \\ 0 & 1 \end{pmatrix}
\]

Therefore, the general formula is:

\[
A^n = \begin{pmatrix} 1 & n \\ 0 & 1 \end{pmatrix}
\]

### 5. Verify the formula for n + 1

Assume that the formula is true for n:

\[
A^n = \begin{pmatrix} 1 & n \\ 0 & 1 \end{pmatrix}
\]

Multiplying both sides by A:

\[
A^{n+1} = A^n \cdot A
\]

\[
A^{n+1} =
\begin{pmatrix} 1 & n \\ 0 & 1 \end{pmatrix}
\begin{pmatrix} 1 & 1 \\ 0 & 1 \end{pmatrix}
\]

\[
A^{n+1} =
\begin{pmatrix}
1 & n+1 \\
0 & 1
\end{pmatrix}
\]

This is exactly the same formula with n replaced by n + 1.

Therefore, the formula holds for all positive integers n.

### Final Answer

\[
\boxed{
A^n = \begin{pmatrix} 1 & n \\ 0 & 1 \end{pmatrix}
}
\]
