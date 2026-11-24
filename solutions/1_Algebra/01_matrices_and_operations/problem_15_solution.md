
# Problem 15 – Associativity of Multiplication and Different Calculation Paths

## Solution

Given:

\[
A = \begin{pmatrix}
1 & 2 & 0 \\
0 & 1 & 1
\end{pmatrix}
\]

\[
B = \begin{pmatrix}
1 & 0 \\
2 & 1 \\
-1 & 3
\end{pmatrix},
\quad
C = \begin{pmatrix}
2 & 1 \\
0 & -1
\end{pmatrix}
\]

### 1. Calculate (AB)C

First, calculate AB.

\[
AB =
\begin{pmatrix}
1 & 2 & 0 \\
0 & 1 & 1
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
1+4+0 & 0+2+0 \\
0+2-1 & 0+1+3
\end{pmatrix}
\]

\[
AB =
\begin{pmatrix}
5 & 2 \\
1 & 4
\end{pmatrix}
\]

Now, multiply AB by C.

\[
(AB)C =
\begin{pmatrix}
5 & 2 \\
1 & 4
\end{pmatrix}
\begin{pmatrix}
2 & 1 \\
0 & -1
\end{pmatrix}
\]

\[
(AB)C =
\begin{pmatrix}
10+0 & 5-2 \\
2+0 & 1-4
\end{pmatrix}
\]

\[
(AB)C =
\begin{pmatrix}
10 & 3 \\
2 & -3
\end{pmatrix}
\]

### 2. Calculate A(BC)

First, calculate BC.

\[
BC =
\begin{pmatrix}
1 & 0 \\
2 & 1 \\
-1 & 3
\end{pmatrix}
\begin{pmatrix}
2 & 1 \\
0 & -1
\end{pmatrix}
\]

\[
BC =
\begin{pmatrix}
2+0 & 1+0 \\
4+0 & 2-1 \\
-2+0 & -1-3
\end{pmatrix}
\]

\[
BC =
\begin{pmatrix}
2 & 1 \\
4 & 1 \\
-2 & -4
\end{pmatrix}
\]

Now, multiply A by BC.

\[
A(BC) =
\begin{pmatrix}
1 & 2 & 0 \\
0 & 1 & 1
\end{pmatrix}
\begin{pmatrix}
2 & 1 \\
4 & 1 \\
-2 & -4
\end{pmatrix}
\]

\[
A(BC) =
\begin{pmatrix}
2+8+0 & 1+2+0 \\
0+4-2 & 0+1-4
\end{pmatrix}
\]

\[
A(BC) =
\begin{pmatrix}
10 & 3 \\
2 & -3
\end{pmatrix}
\]

### 3. Compare the results

We obtained:

\[
(AB)C =
\begin{pmatrix}
10 & 3 \\
2 & -3
\end{pmatrix}
\]

\[
A(BC) =
\begin{pmatrix}
10 & 3 \\
2 & -3
\end{pmatrix}
\]

Therefore,

\[
\boxed{(AB)C = A(BC)}
\]

Both calculation paths give exactly the same result.

### 4. Compare the number of operations

In the first calculation path:

- Calculate AB (2 × 3 multiplied by 3 × 2).
- Multiply the result by C (2 × 2 multiplied by 2 × 2).

In the second calculation path:

- Calculate BC (3 × 2 multiplied by 2 × 2).
- Multiply A by the result (2 × 3 multiplied by 3 × 2).

Both paths require two matrix multiplications and one intermediate matrix.

However, the first path requires 20 scalar multiplications, while the second path requires 24 scalar multiplications.

Therefore, calculating (AB)C requires fewer scalar multiplications in this example.

### 5. Explanation

Associativity means that the grouping of matrix multiplication does not change the final result.

Although the intermediate matrices are different, both calculation paths produce the same final matrix.

This property is expressed as:

\[
(AB)C = A(BC)
\]

It is important to note that associativity does not mean that matrix multiplication is commutative.

### Final Answer

\[
\boxed{
(AB)C = A(BC) =
\begin{pmatrix}
10 & 3 \\
2 & -3
\end{pmatrix}
}
\]

Matrix multiplication is associative because changing the grouping of the matrices does not change the final result.
