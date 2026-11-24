
# Problem 04 – Matrix Multiplication and Noncommutativity

## Solution

Given:

\[
A = \begin{pmatrix} 1 & 2 \\ 0 & 1 \end{pmatrix},
\quad
B = \begin{pmatrix} 2 & 0 \\ 3 & 1 \end{pmatrix}
\]

### 1. Calculate AB

We multiply each row of A by each column of B.

\[
AB =
\begin{pmatrix}
1\cdot2+2\cdot3 & 1\cdot0+2\cdot1 \\
0\cdot2+1\cdot3 & 0\cdot0+1\cdot1
\end{pmatrix}
\]

\[
AB =
\begin{pmatrix}
8 & 2 \\
3 & 1
\end{pmatrix}
\]

### 2. Calculate BA

Now we multiply B by A.

\[
BA =
\begin{pmatrix}
2\cdot1+0\cdot0 & 2\cdot2+0\cdot1 \\
3\cdot1+1\cdot0 & 3\cdot2+1\cdot1
\end{pmatrix}
\]

\[
BA =
\begin{pmatrix}
2 & 4 \\
3 & 7
\end{pmatrix}
\]

### 3. Compare AB and BA

\[
AB =
\begin{pmatrix} 8 & 2 \\ 3 & 1 \end{pmatrix}
\]

\[
BA =
\begin{pmatrix} 2 & 4 \\ 3 & 7 \end{pmatrix}
\]

Therefore,

\[
AB \neq BA
\]

### 4. Explanation

Matrix multiplication is not commutative because changing the order of the matrices can produce different results.

In this example, AB and BA have different entries.

This property is called noncommutativity.

### Final Answer

\[
\boxed{AB \neq BA}
\]

Matrix multiplication does not generally satisfy the commutative property.
