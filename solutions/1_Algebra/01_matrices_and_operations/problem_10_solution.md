### Exercise 10. Inverse of a $2 \times 2$ Matrix

**Problem:**

For

$$
A = \begin{pmatrix}
2 & 1 \\
5 & 3
\end{pmatrix}
$$

compute its determinant, find its inverse matrix $A^{-1}$, and verify that $A A^{-1} = I$ and $A^{-1} A = I$.

---

## Solution

### 1. Computing the Determinant

For a $2 \times 2$ matrix $A = \begin{pmatrix} a & b \\ c & d \end{pmatrix}$, the determinant is given by $\det(A) = ad - bc$.

$$
\det(A) = (2)(3) - (1)(5) = 6 - 5 = 1
$$

Since $\det(A) \neq 0$, the matrix $A$ is invertible.

### 2. Finding the Inverse Matrix $A^{-1}$

The inverse of a $2 \times 2$ matrix is given by:

$$
A^{-1} = \frac{1}{\det(A)} \begin{pmatrix}
d & -b \\
-c & a
\end{pmatrix}
$$

Substituting the values:

$$
A^{-1} = \frac{1}{1} \begin{pmatrix}
3 & -1 \\
-5 & 2
\end{pmatrix}
= \begin{pmatrix}
3 & -1 \\
-5 & 2
\end{pmatrix}
$$

### 3. Verification ($A A^{-1} = I$ and $A^{-1} A = I$)

To verify, we compute the product $A A^{-1}$:

$$
A A^{-1} = \begin{pmatrix}
2 & 1 \\
5 & 3
\end{pmatrix}
\begin{pmatrix}
3 & -1 \\
-5 & 2
\end{pmatrix}
= \begin{pmatrix}
(2)(3) + (1)(-5) & (2)(-1) + (1)(2) \\
(5)(3) + (3)(-5) & (5)(-1) + (3)(2)
\end{pmatrix}
$$

Simplifying each entry:

$$
A A^{-1} = \begin{pmatrix}
6 - 5 & -2 + 2 \\
15 - 15 & -5 + 6
\end{pmatrix}
= \begin{pmatrix}
1 & 0 \\
0 & 1
\end{pmatrix} = I
$$

Next, we compute the product $A^{-1} A$:

$$
A^{-1} A = \begin{pmatrix}
3 & -1 \\
-5 & 2
\end{pmatrix}
\begin{pmatrix}
2 & 1 \\
5 & 3
\end{pmatrix}
= \begin{pmatrix}
(3)(2) + (-1)(5) & (3)(1) + (-1)(3) \\
(-5)(2) + (2)(5) & (-5)(1) + (2)(3)
\end{pmatrix}
$$

Simplifying each entry:

$$
A^{-1} A = \begin{pmatrix}
6 - 5 & 3 - 3 \\
-10 + 10 & -5 + 6
\end{pmatrix}
= \begin{pmatrix}
1 & 0 \\
0 & 1
\end{pmatrix} = I
$$

Both products yield the identity matrix $I$, confirming that the computed inverse is correct.

 



  
