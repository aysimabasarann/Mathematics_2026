### Exercise 5. Matrix Times Vector

**Problem:**

Let

$$
A = \begin{pmatrix}
2 & -1 \\
1 & 3
\end{pmatrix}
$$

and

$$
x = \begin{pmatrix}
4 \\
2
\end{pmatrix}
$$

Compute $Ax$. Then express $Ax$ as a linear combination of the columns of $A$, with coefficients coming from the vector $x$.

---

## Solution

### 1. Computing the Matrix-Vector Product $Ax$

To compute $Ax$, we take the dot product of each row of $A$ with the vector $x$:

$$
Ax = \begin{pmatrix}
2 & -1 \\
1 & 3
\end{pmatrix}
\begin{pmatrix}
4 \\
2
\end{pmatrix}
= \begin{pmatrix}
(2)(4) + (-1)(2) \\
(1)(4) + (3)(2)
\end{pmatrix}
= \begin{pmatrix}
8 - 2 \\
4 + 6
\end{pmatrix}
= \begin{pmatrix}
6 \\
10
\end{pmatrix}
$$

### 2. Expressing $Ax$ as a Linear Combination of Columns

A fundamental property of matrix-vector multiplication is that the product $Ax$ can be viewed as a linear combination of the columns of matrix $A$, where the scalars (coefficients) are the entries of the vector $x$.

Letting $a_1$ and $a_2$ be the columns of $A$:

$$
a_1 = \begin{pmatrix}
2 \\
1
\end{pmatrix}, \qquad a_2 = \begin{pmatrix}
-1 \\
3
\end{pmatrix}
$$

Using the entries of $x = \begin{pmatrix} 4 \\ 2 \end{pmatrix}$ as coefficients:

$$
Ax = 4 \cdot a_1 + 2 \cdot a_2 = 4 \begin{pmatrix}
2 \\
1
\end{pmatrix} + 2 \begin{pmatrix}
-1 \\
3
\end{pmatrix}
$$

Calculating this expression:

$$
4 \begin{pmatrix}
2 \\
1
\end{pmatrix} + 2 \begin{pmatrix}
-1 \\
3
\end{pmatrix} = \begin{pmatrix}
8 \\
4
\end{pmatrix} + \begin{pmatrix}
-2 \\
6
\end{pmatrix} = \begin{pmatrix}
8 - 2 \\
4 + 6
\end{pmatrix} = \begin{pmatrix}
6 \\
10
\end{pmatrix}
$$

Both methods yield the same result, confirming that matrix-vector multiplication is equivalent to a linear combination of the matrix columns.

