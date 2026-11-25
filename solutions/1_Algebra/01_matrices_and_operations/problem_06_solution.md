### Exercise 6. Transpose

**Problem:**

For

$$
A = \begin{pmatrix}
1 & 2 & 3 \\
4 & 5 & 6
\end{pmatrix}
$$

and

$$
B = \begin{pmatrix}
1 & 0 \\
2 & 1 \\
-1 & 3
\end{pmatrix}
$$

compute $A^T$, $B^T$, and $AB$. Then verify in this example that

$$
(AB)^T = B^T A^T.
$$

---

## Solution

### 1. Computing Transposes $A^T$ and $B^T$

The transpose of a matrix is formed by swapping its rows and columns:

$$
A^T = \begin{pmatrix}
1 & 4 \\
2 & 5 \\
3 & 6
\end{pmatrix}
$$

$$
B^T = \begin{pmatrix}
1 & 2 & -1 \\
0 & 1 & 3
\end{pmatrix}
$$

### 2. Computing the Product $AB$

Matrix $A$ is of size $2 \times 3$ and matrix $B$ is of size $3 \times 2$, so their product $AB$ is a $2 \times 2$ matrix:

$$
AB = \begin{pmatrix}
1 & 2 & 3 \\
4 & 5 & 6
\end{pmatrix}
\begin{pmatrix}
1 & 0 \\
2 & 1 \\
-1 & 3
\end{pmatrix}
= \begin{pmatrix}
(1)(1) + (2)(2) + (3)(-1) & (1)(0) + (2)(1) + (3)(3) \\
(4)(1) + (5)(2) + (6)(-1) & (4)(0) + (5)(1) + (6)(3)
\end{pmatrix}
$$

Simplifying each entry:

$$
AB = \begin{pmatrix}
1 + 4 - 3 & 0 + 2 + 9 \\
4 + 10 - 6 & 0 + 5 + 18
\end{pmatrix}
= \begin{pmatrix}
2 & 11 \\
8 & 23
\end{pmatrix}
$$

### 3. Transposing the Product: $(AB)^T$

Taking the transpose of the resulting product matrix $AB$:

$$
(AB)^T = \begin{pmatrix}
2 & 8 \\
11 & 23
\end{pmatrix}
$$

### 4. Computing the Product $B^T A^T$

Matrix $B^T$ is of size $2 \times 3$ and matrix $A^T$ is of size $3 \times 2$, so their product $B^T A^T$ is a $2 \times 2$ matrix:

$$
B^T A^T = \begin{pmatrix}
1 & 2 & -1 \\
0 & 1 & 3
\end{pmatrix}
\begin{pmatrix}
1 & 4 \\
2 & 5 \\
3 & 6
\end{pmatrix}
= \begin{pmatrix}
(1)(1) + (2)(2) + (-1)(3) & (1)(4) + (2)(5) + (-1)(6) \\
(0)(1) + (1)(2) + (3)(3) & (0)(4) + (1)(5) + (3)(6)
\end{pmatrix}
$$

Simplifying each entry:

$$
B^T A^T = \begin{pmatrix}
1 + 4 - 3 & 4 + 10 - 6 \\
0 + 2 + 9 & 0 + 5 + 18
\end{pmatrix}
= \begin{pmatrix}
2 & 8 \\
11 & 23
\end{pmatrix}
$$

### 5. Verification

Comparing the results from sections 3 and 4, we observe that:

$$
(AB)^T = \begin{pmatrix}
2 & 8 \\
11 & 23
\end{pmatrix}
= B^T A^T
$$

Thus, the property $(AB)^T = B^T A^T$ is successfully verified for this example.

