### Exercise 6. Parameter and Invertibility

For

$$
A(t)=
\begin{pmatrix}
t & 1 \\
2 & t \\
\end{pmatrix}
$$

find all values of $t$ for which the matrix is not invertible. Explain how your answer is related to the determinant being zero.

---

## Solution

### 1. Computing the Determinant in Terms of $t$

For the $2 \times 2$ matrix $A(t)$, we compute its determinant using the standard formula $ad - bc$:

$$
\det A(t) = (t)(t) - (1)(2) = t^2 - 2
$$

### 2. Finding Values of $t$ for Which the Matrix Is Not Invertible

A square matrix is not invertible if and only if its determinant is equal to zero. Setting our determinant expression to zero gives:

$$
t^2 - 2 = 0
$$

Solving for $t$:

$$
t^2 = 2 \implies t = \pm\sqrt{2}
$$

### 3. Explanation

**Relationship with the Determinant:**
The inverse of a $2 \times 2$ matrix $A = \begin{pmatrix} a & b \\ c & d \end{pmatrix}$ involves dividing by its determinant ($\det A = ad - bc$). If the determinant is zero, division by zero is undefined, and the inverse matrix does not exist. 

Therefore, for $t = \sqrt{2}$ and $t = -\sqrt{2}$, the matrix $A(t)$ has a determinant of zero and is thus **not invertible**. For any other real value of $t$, the determinant is non-zero, making the matrix invertible.

 
