### Exercise 2. Formula for a $2\times2$ Matrix

Find the inverse of

$$
A=
\begin{pmatrix}
3 & 2 \\
5 & 4 \\
\end{pmatrix}
$$

using the formula for a $2\times2$ matrix. At the end, check the result by computing one product with $A$.

---

## Solution

### 1. Applying the Inverse Formula for a $2 \times 2$ Matrix

For a general $2 \times 2$ matrix

$$
M =
\begin{pmatrix}
a & b \\
c & d \\
\end{pmatrix}
$$

the inverse matrix $M^{-1}$ exists if and only if $\det M = ad - bc \neq 0$, and is given by the formula:

$$
M^{-1} = \frac{1}{ad - bc}
\begin{pmatrix}
d & -b \\
-c & a \\
\end{pmatrix}
$$

For the given matrix $A$, we identify the entries $a = 3$, $b = 2$, $c = 5$, and $d = 4$. First, we compute the determinant of $A$:

$$
\det A = (3)(4) - (2)(5) = 12 - 10 = 2
$$

Since $\det A = 2 \neq 0$, the inverse $A^{-1}$ exists. Substituting the entries and the determinant into the formula yields:

$$
\begin{aligned}
A^{-1} &= \frac{1}{2}
\begin{pmatrix}
4 & -2 \\
-5 & 3 \\
\end{pmatrix} \\
&=
\begin{pmatrix}
2 & -1 \\
-\frac{5}{2} & \frac{3}{2} \\
\end{pmatrix}
\end{aligned}
$$

### 2. Verification by Multiplication

To verify that this matrix is indeed $A^{-1}$, we compute the product $AA^{-1}$:

$$
\begin{aligned}
AA^{-1} &=
\begin{pmatrix}
3 & 2 \\
5 & 4 \\
\end{pmatrix}
\begin{pmatrix}
2 & -1 \\
-\frac{5}{2} & \frac{3}{2} \\
\end{pmatrix} \\
&=
\begin{pmatrix}
(3)(2) + (2)\left(-\frac{5}{2}\right) & (3)(-1) + (2)\left(\frac{3}{2}\right) \\
(5)(2) + (4)\left(-\frac{5}{2}\right) & (5)(-1) + (4)\left(\frac{3}{2}\right) \\
\end{pmatrix} \\
&=
\begin{pmatrix}
6 - 5 & -3 + 3 \\
10 - 10 & -5 + 6 \\
\end{pmatrix} \\
&=
\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix}
= I
\end{aligned}
$$

Since $AA^{-1} = I$, the computed inverse is verified.




