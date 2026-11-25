### Exercise 10. Inverse of a Diagonal Matrix

Given

$$
D=
\begin{pmatrix}
2 & 0 & 0 \\
0 & -3 & 0 \\
0 & 0 & 5 \\
\end{pmatrix},\qquad E=
\begin{pmatrix}
2 & 0 & 0 \\
0 & 0 & 0 \\
0 & 0 & 5 \\
\end{pmatrix}
$$

Without using Gauss–Jordan elimination, decide which matrix is invertible. For the invertible matrix, give the inverse and check the result by multiplication.

---

## Solution

### 1. Determining Which Matrix Is Invertible

A diagonal matrix is invertible if and only if all of its main diagonal entries are nonzero, because the determinant of a diagonal matrix is the product of its diagonal entries.

For matrix $D$, the diagonal entries are $2$, $-3$, and $5$. Since none of these entries is zero:

$$
\det D = (2)(-3)(5) = -30 \neq 0
$$

Thus, matrix $D$ is invertible.

For matrix $E$, the second diagonal entry is $0$ (entire second row is zero), which makes its determinant zero:

$$
\det E = (2)(0)(5) = 0
$$

Therefore, matrix $E$ is not invertible.

### 2. Finding the Inverse Matrix $D^{-1}$

The inverse of an invertible diagonal matrix is obtained directly by taking the reciprocal of each main diagonal entry:

$$
D^{-1} =
\begin{pmatrix}
\frac{1}{2} & 0 & 0 \\
0 & -\frac{1}{3} & 0 \\
0 & 0 & \frac{1}{5} \\
\end{pmatrix}
$$

### 3. Verification by Multiplication

To check the result, we compute the product $DD^{-1}$:

$$
DD^{-1} =
\begin{pmatrix}
2 & 0 & 0 \\
0 & -3 & 0 \\
0 & 0 & 5 \\
\end{pmatrix}
\begin{pmatrix}
\frac{1}{2} & 0 & 0 \\
0 & -\frac{1}{3} & 0 \\
0 & 0 & \frac{1}{5} \\
\end{pmatrix}
$$

Multiplying the corresponding diagonal entries:

$$
DD^{-1} =
\begin{pmatrix}
(2)\left(\frac{1}{2}\right) & 0 & 0 \\
0 & (-3)\left(-\frac{1}{3}\right) & 0 \\
0 & 0 & (5)\left(\frac{1}{5}\right) \\
\end{pmatrix}
$$

Simplifying each entry:

$$
DD^{-1} =
\begin{pmatrix}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1 \\
\end{pmatrix}
= I
$$

Since $DD^{-1} = I$, the inverse matrix $D^{-1}$ is verified[span_0](start_span)[span_0](end_span).


 




 
