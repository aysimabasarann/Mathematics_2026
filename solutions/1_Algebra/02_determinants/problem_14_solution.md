 ### Exercise 14. Cofactor Expansion

Compute the determinant

$$
A=
\begin{pmatrix}
2 & 0 & 1 \\
3 & 5 & 0 \\
1 & 4 & -2 \\
\end{pmatrix}
$$

by expanding along the first row. Then verify your result by expanding along the second column.

---

## Solution

### 1. Expansion Along the First Row

The cofactor expansion of a $3 \times 3$ matrix along its first row is given by:

$$
\det A = a_{11} C_{11} + a_{12} C_{12} + a_{13} C_{13}
$$

where the cofactors are $C_{ij} = (-1)^{i+j} M_{ij}$, and $M_{ij}$ is the determinant of the $2 \times 2$ submatrix obtained by removing the $i$-th row and $j$-th column.

For our matrix, the first row entries are $a_{11} = 2$, $a_{12} = 0$, and $a_{13} = 1$. We evaluate each term separately:

**First term ($a_{11} C_{11}$):**

$$
2 \cdot (-1)^{1+1} \det \begin{pmatrix} 5 & 0 \\ 4 & -2 \end{pmatrix} = 2 \cdot 1 \cdot ((5)(-2) - (0)(4)) = 2(-10) = -20
$$

**Second term ($a_{12} C_{12}$):**

$$
0 \cdot (-1)^{1+2} \det \begin{pmatrix} 3 & 0 \\ 1 & -2 \end{pmatrix} = 0
$$

**Third term ($a_{13} C_{13}$):**

$$
1 \cdot (-1)^{1+3} \det \begin{pmatrix} 3 & 5 \\ 1 & 4 \end{pmatrix} = 1 \cdot 1 \cdot ((3)(4) - (5)(1)) = 1(12 - 5) = 7
$$

Summing these terms yields the determinant:

$$
\det A = -20 + 0 + 7 = -13
$$

### 2. Verification by Expanding Along the Second Column

The entries of the second column are $a_{12} = 0$, $a_{22} = 5$, and $a_{32} = 4$, with signs given by $(-1)^{i+2}$ ($-$, $+$, $-$):

$$
\det A = -a_{12} M_{12} + a_{22} M_{22} - a_{32} M_{32}
$$

Evaluating each term:

**First term ($a_{12} = 0$):**

$$
-0 \cdot \det \begin{pmatrix} 3 & 0 \\ 1 & -2 \end{pmatrix} = 0
$$

**Second term ($a_{22} = 5$):**

$$
5 \cdot \det \begin{pmatrix} 2 & 1 \\ 1 & -2 \end{pmatrix} = 5 \cdot ((2)(-2) - (1)(1)) = 5(-4 - 1) = 5(-5) = -25
$$

**Third term ($a_{32} = 4$):**

$$
-4 \cdot \det \begin{pmatrix} 2 & 1 \\ 3 & 0 \end{pmatrix} = -4 \cdot ((2)(0) - (1)(3)) = -4(0 - 3) = -4(-3) = 12
$$

Summing these terms gives:

$$
\det A = 0 - 25 + 12 = -13
$$

Both methods yield $-13$, confirming our result.


