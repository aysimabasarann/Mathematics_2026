### Exercise 11. Parameter and Invertibility

For

$$
A(t)=
\begin{pmatrix}
1 & t \\
t & 1 \\
\end{pmatrix}
$$

find all $t$ for which the matrix is invertible, and then give a formula for $A(t)^{-1}$. Explain what happens to this formula at the excluded values.

---

## Solution

### 1. Finding All $t$ for Which $A(t)$ Is Invertible

A square matrix is invertible if and only if its determinant is nonzero. We compute the determinant of $A(t)$:

$$
\det A(t) = (1)(1) - (t)(t) = 1 - t^2
$$

To find the values of $t$ for which the matrix is not invertible, we set the determinant equal to zero:

$$
1 - t^2 = 0
$$

Factoring the difference of squares gives:

$$
(1 - t)(1 + t) = 0
$$

This yields two excluded values: $t = 1$ and $t = -1$. 

Therefore, $A(t)$ is invertible for all real numbers $t \neq 1$ and $t \neq -1$ (i.e., $t \in \mathbb{R} \setminus \{-1, 1\}$).

### 2. Formula for $A(t)^{-1}$

For any $t \neq \pm 1$, we apply the $2 \times 2$ inverse formula using $\det A(t) = 1 - t^2$:

$$
A(t)^{-1} = \frac{1}{1 - t^2}
\begin{pmatrix}
1 & -t \\
-t & 1 \\
\end{pmatrix}
$$

Distributing the scalar factor into each entry gives:

$$
A(t)^{-1} =
\begin{pmatrix}
\frac{1}{1 - t^2} & -\frac{t}{1 - t^2} \\
-\frac{t}{1 - t^2} & \frac{1}{1 - t^2} \\
\end{pmatrix}
$$

### 3. Behavior at the Excluded Values

At the excluded values $t = 1$ and $t = -1$, the denominator $1 - t^2$ in the inverse formula becomes zero, resulting in division by zero, which is undefined.

Geometrically and algebraically, at $t = 1$ the matrix becomes

$$
A(1) =
\begin{pmatrix}
1 & 1 \\
1 & 1 \\
\end{pmatrix}
$$

and at $t = -1$ the matrix becomes

$$
A(-1) =
\begin{pmatrix}
1 & -1 \\
-1 & 1 \\
\end{pmatrix}
$$

In both cases, the rows of the matrix are linearly dependent (either identical or scalar multiples of $-1$), meaning the transformation collapses the plane onto a line and cannot be reversed.



