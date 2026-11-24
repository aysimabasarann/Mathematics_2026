
# Problem 13 – A Recurrence Written in Matrix Form

## Solution

Given:

\[
F = \begin{pmatrix} 1 & 1 \\ 1 & 0 \end{pmatrix}
\]

### 1. Calculate F²

\[
F^2 = F \cdot F
\]

\[
F^2 =
\begin{pmatrix} 1 & 1 \\ 1 & 0 \end{pmatrix}
\begin{pmatrix} 1 & 1 \\ 1 & 0 \end{pmatrix}
\]

\[
F^2 =
\begin{pmatrix}
1+1 & 1+0 \\
1+0 & 1+0
\end{pmatrix}
\]

\[
F^2 = \begin{pmatrix} 2 & 1 \\ 1 & 1 \end{pmatrix}
\]

### 2. Calculate F³

\[
F^3 = F^2 \cdot F
\]

\[
F^3 =
\begin{pmatrix} 2 & 1 \\ 1 & 1 \end{pmatrix}
\begin{pmatrix} 1 & 1 \\ 1 & 0 \end{pmatrix}
\]

\[
F^3 =
\begin{pmatrix}
2+1 & 2+0 \\
1+1 & 1+0
\end{pmatrix}
\]

\[
F^3 = \begin{pmatrix} 3 & 2 \\ 2 & 1 \end{pmatrix}
\]

### 3. Calculate F⁴

\[
F^4 = F^3 \cdot F
\]

\[
F^4 =
\begin{pmatrix} 3 & 2 \\ 2 & 1 \end{pmatrix}
\begin{pmatrix} 1 & 1 \\ 1 & 0 \end{pmatrix}
\]

\[
F^4 =
\begin{pmatrix}
3+2 & 3+0 \\
2+1 & 2+0
\end{pmatrix}
\]

\[
F^4 = \begin{pmatrix} 5 & 3 \\ 3 & 2 \end{pmatrix}
\]

### 4. Calculate F⁵

\[
F^5 = F^4 \cdot F
\]

\[
F^5 =
\begin{pmatrix} 5 & 3 \\ 3 & 2 \end{pmatrix}
\begin{pmatrix} 1 & 1 \\ 1 & 0 \end{pmatrix}
\]

\[
F^5 =
\begin{pmatrix}
5+3 & 5+0 \\
3+2 & 3+0
\end{pmatrix}
\]

\[
F^5 = \begin{pmatrix} 8 & 5 \\ 5 & 3 \end{pmatrix}
\]

### 5. Compare with the Fibonacci sequence

The Fibonacci sequence is:

\[
0,1,1,2,3,5,8,\ldots
\]

The calculated matrices are:

\[
F^2 = \begin{pmatrix} 2 & 1 \\ 1 & 1 \end{pmatrix}
\]

\[
F^3 = \begin{pmatrix} 3 & 2 \\ 2 & 1 \end{pmatrix}
\]

\[
F^4 = \begin{pmatrix} 5 & 3 \\ 3 & 2 \end{pmatrix}
\]

\[
F^5 = \begin{pmatrix} 8 & 5 \\ 5 & 3 \end{pmatrix}
\]

We can see that the entries of these matrices are consecutive Fibonacci numbers.

### 6. Calculate F(a, b)

We multiply the matrix F by the vector:

\[
F\begin{pmatrix} a \\ b \end{pmatrix}
=
\begin{pmatrix} 1 & 1 \\ 1 & 0 \end{pmatrix}
\begin{pmatrix} a \\ b \end{pmatrix}
\]

\[
=
\begin{pmatrix}
a+b \\
a
\end{pmatrix}
\]

### 7. Explanation

The multiplication creates the sum of two consecutive terms and keeps the first term for the next step.

The new vector is:

\[
\begin{pmatrix} a+b \\ a \end{pmatrix}
\]

This follows the Fibonacci recurrence:

\[
F_{n+1}=F_n+F_{n-1}
\]

Therefore, matrix multiplication performs one step of the Fibonacci sequence.

### Final Answer

\[
F^2 = \begin{pmatrix} 2 & 1 \\ 1 & 1 \end{pmatrix}
\]

\[
F^3 = \begin{pmatrix} 3 & 2 \\ 2 & 1 \end{pmatrix}
\]

\[
F^4 = \begin{pmatrix} 5 & 3 \\ 3 & 2 \end{pmatrix}
\]

\[
F^5 = \begin{pmatrix} 8 & 5 \\ 5 & 3 \end{pmatrix}
\]

\[
\boxed{
F\begin{pmatrix} a \\ b \end{pmatrix}
=
\begin{pmatrix} a+b \\ a \end{pmatrix}
}
\]

The matrix F generates consecutive Fibonacci numbers through repeated matrix multiplication.
