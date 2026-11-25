### Exercise 14. A Matrix That Is Its Own Inverse

Assume that a square matrix $A$ satisfies

$$
A^2=I.
$$

Show that

$$
A^{-1}=A.
$$

Then give an example of a $2\times2$ matrix different from $I$ and $-I$ that satisfies this condition, and verify it by multiplication.

---

## Solution

### 1. Proof That $A^{-1} = A$

By definition, a square matrix $B$ is the inverse of $A$ if and only if $AB = BA = I$.

We are given that $A^2 = I$, which can be written as:

$$
A \cdot A = I
$$

Comparing this directly with the definition of the inverse matrix ($A \cdot A^{-1} = I$), we see that $A$ itself plays the role of $A^{-1}$.

Alternatively, we can verify that $A$ is invertible by taking the determinant of both sides:

$$
\det(A^2) = \det(I)
$$

Using the determinant property $\det(A^2) = (\det A)^2$ and $\det I = 1$:

$$
(\det A)^2 = 1 \implies \det A = \pm 1 \neq 0
$$

Since $\det A \neq 0$, the inverse matrix $A^{-1}$ exists. Multiplying both sides of $A^2 = I$ by $A^{-1}$ gives:

$$
A^{-1}(A^2) = A^{-1}I
$$

Using the associative property $(A^{-1}A)A = IA$:

$$
A = A^{-1}
$$

Thus, $A^{-1} = A$.

### 2. Example of a Nontrivial $2 \times 2$ Matrix

Consider the reflection matrix across the $x$-axis, which is different from both $I$ and $-I$:

$$
A =
\begin{pmatrix}
1 & 0 \\
0 & -1 \\
\end{pmatrix}
$$

### 3. Verification by Multiplication

We compute $A^2$ to verify that $A^2 = I$:

$$
A^2 =
\begin{pmatrix}
1 & 0 \\
0 & -1 \\
\end{pmatrix}
\begin{pmatrix}
1 & 0 \\
0 & -1 \\
\end{pmatrix}
$$

Writing out the multiplication of entries:

$$
A^2 =
\begin{pmatrix}
(1)(1) + (0)(0) & (1)(0) + (0)(-1) \\
(0)(1) + (-1)(0) & (0)(0) + (-1)(-1) \\
\end{pmatrix}
$$

Simplifying the entries:

$$
A^2 =
\begin{pmatrix}
1 + 0 & 0 + 0 \\
0 + 0 & 0 + 1 \\
\end{pmatrix}
$$

Evaluating the sums:

$$
A^2 =
\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix}
= I
$$

Since $A^2 = I$, this matrix satisfies the condition and is its own inverse ($A^{-1} = A$).

  
