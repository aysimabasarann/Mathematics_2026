### Exercise 1. Determinant of a 2×2 Matrix

Compute

$$
\det
\begin{pmatrix}
3 & -2 \\
5 & 4 \\
\end{pmatrix},\qquad \det
\begin{pmatrix}
1 & 7 \\
2 & 14 \\
\end{pmatrix}.
$$

Which matrix is invertible? Justify your answer.

---

## Solution

### 1. Computing the Determinants

For any $2 \times 2$ matrix of the form

$$
A = \begin{pmatrix}
a & b \\
c & d
\end{pmatrix}
$$

the determinant is computed using the formula:

$$
\det(A) = ad - bc
$$

Applying this formula to the first matrix:

$$
\det
\begin{pmatrix}
3 & -2 \\
5 & 4 \\
\end{pmatrix}
= (3)(4) - (-2)(5) = 12 - (-10) = 12 + 10 = 22
$$

Applying the formula to the second matrix:

$$
\det
\begin{pmatrix}
1 & 7 \\
2 & 14 \\
\end{pmatrix}
= (1)(14) - (7)(2) = 14 - 14 = 0
$$

### 2. Invertibility Justification

A square matrix is invertible if and only if its determinant is non-zero ($\det(A) \neq 0$).

* The first matrix has a determinant of $22$, which is non-zero. Therefore, **the first matrix is invertible**.
* The second matrix has a determinant of $0$. Therefore, **the second matrix is not invertible**.

 
