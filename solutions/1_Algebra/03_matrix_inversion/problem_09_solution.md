### Exercise 9. Matrix Equation

Given

$$
A=
\begin{pmatrix}
1 & 2 \\
0 & 1 \\
\end{pmatrix},\qquad B=
\begin{pmatrix}
3 & 1 \\
2 & 4 \\
\end{pmatrix}
$$

Solve the equation $AX=B$ for $X$. Before calculating, decide on which side of the equation $A^{-1}$ must be used. Then check the result by computing $AX$.

---

## Solution

### 1. Determining the Side for $A^{-1}$

We are given the matrix equation:

$$
AX = B
$$

To isolate the unknown matrix $X$, we must eliminate matrix $A$ from the left side. Since matrix multiplication is not commutative, the placement matters. By multiplying both sides on the left by $A^{-1}$, we get:

$$
A^{-1}(AX) = A^{-1}B
$$

Using the associative property of matrix multiplication ($A^{-1}A = I$):

$$
IX = A^{-1}B \implies X = A^{-1}B
$$

Thus, $A^{-1}$ must be used on the **left side** of $B$.

### 2. Finding $A^{-1}$

First, we compute the determinant of $A$:

$$
\det A = (1)(1) - (2)(0) = 1 - 0 = 1
$$

Since $\det A = 1 \neq 0$, $A$ is invertible. Applying the $2 \times 2$ inverse formula:

$$
A^{-1} = \frac{1}{1}
\begin{pmatrix}
1 & -2 \\
0 & 1 \\
\end{pmatrix}
$$

Simplifying the matrix:

$$
A^{-1} =
\begin{pmatrix}
1 & -2 \\
0 & 1 \\
\end{pmatrix}
$$

### 3. Computing the Solution Matrix $X$

Now we compute $X = A^{-1}B$ by multiplying the matrices:

$$
X =
\begin{pmatrix}
1 & -2 \\
0 & 1 \\
\end{pmatrix}
\begin{pmatrix}
3 & 1 \\
2 & 4 \\
\end{pmatrix}
$$

Writing out the multiplication of entries:

$$
X =
\begin{pmatrix}
(1)(3) + (-2)(2) & (1)(1) + (-2)(4) \\
(0)(3) + (1)(2) & (0)(1) + (1)(4) \\
\end{pmatrix}
$$

Simplifying the entries:

$$
X =
\begin{pmatrix}
3 - 4 & 1 - 8 \\
0 + 2 & 0 + 4 \\
\end{pmatrix}
$$

Evaluating the sums:

$$
X =
\begin{pmatrix}
-1 & -7 \\
2 & 4 \\
\end{pmatrix}
$$

### 4. Verification by Computing $AX$

To check our result, we compute the product $AX$ and verify that it equals $B$:

$$
AX =
\begin{pmatrix}
1 & 2 \\
0 & 1 \\
\end{pmatrix}
\begin{pmatrix}
-1 & -7 \\
2 & 4 \\
\end{pmatrix}
$$

Writing out the multiplication:

$$
AX =
\begin{pmatrix}
(1)(-1) + (2)(2) & (1)(-7) + (2)(4) \\
(0)(-1) + (1)(2) & (0)(-7) + (1)(4) \\
\end{pmatrix}
$$

Simplifying the entries:

$$
AX =
\begin{pmatrix}
-1 + 4 & -7 + 8 \\
0 + 2 & 0 + 4 \\
\end{pmatrix}
$$

Evaluating the sums:

$$
AX =
\begin{pmatrix}
3 & 1 \\
2 & 4 \\
\end{pmatrix}
= B
$$

Since $AX = B$ holds true, the solution matrix $X$ is verified.

 


