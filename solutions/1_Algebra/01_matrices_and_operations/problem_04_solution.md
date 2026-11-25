### Exercise 4. Matrix Multiplication and Noncommutativity

**Problem:**

For

$$
A = \begin{pmatrix}
1 & 2 \\
0 & 1
\end{pmatrix}
$$

and

$$
B = \begin{pmatrix}
2 & 0 \\
3 & 1
\end{pmatrix}
$$

compute $AB$ and $BA$. Is $AB=BA$? Use this example to explain what noncommutativity of matrix multiplication means.

---

## Solution

### 1. Computing the Product $AB$

To find $AB$, we compute the dot products of the rows of $A$ with the columns of $B$:

$$
AB = \begin{pmatrix}
1 & 2 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
2 & 0 \\
3 & 1
\end{pmatrix}
= \begin{pmatrix}
(1)(2) + (2)(3) & (1)(0) + (2)(1) \\
(0)(2) + (1)(3) & (0)(0) + (1)(1)
\end{pmatrix}
= \begin{pmatrix}
8 & 2 \\
3 & 1
\end{pmatrix}
$$

### 2. Computing the Product $BA$

To find $BA$, we multiply the rows of $B$ by the columns of $A$:

$$
BA = \begin{pmatrix}
2 & 0 \\
3 & 1
\end{pmatrix}
\begin{pmatrix}
1 & 2 \\
0 & 1
\end{pmatrix}
= \begin{pmatrix}
(2)(1) + (0)(0) & (2)(2) + (0)(1) \\
(3)(1) + (1)(0) & (3)(2) + (1)(1)
\end{pmatrix}
= \begin{pmatrix}
2 & 4 \\
3 & 7
\end{pmatrix}
$$

### 3. Comparison and Noncommutativity

Comparing the results, we find that:

$$
AB = \begin{pmatrix}
8 & 2 \\
3 & 1
\end{pmatrix}
\neq
\begin{pmatrix}
2 & 4 \\
3 & 7
\end{pmatrix}
= BA
$$

Therefore, $AB \neq BA$. 

**Explanation of Noncommutativity:** 
In ordinary arithmetic, multiplication is commutative, meaning that the order of factors does not change the product ($ab = ba$). In matrix algebra, matrix multiplication is generally **noncommutative**. This means that changing the order in which matrices are multiplied typically yields completely different results, and in many cases, even if both products $AB$ and $BA$ are defined, they are not equal.




