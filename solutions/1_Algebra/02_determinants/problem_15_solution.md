

# Exercise 15. Combining Determinant Properties

Let $A$ and $B$ be invertible $2 \times 2$ matrices with

$$
\det A = -2, \qquad \det B = 3.
$$

Without finding the entries of the matrices, compute

$$
\det\left(B^{-1} A^T B\right).
$$

State the determinant properties you use in order and explain why the factors involving $B$ eventually cancel.

---

## Solution

**1. Determinant Properties Used in Order**

To evaluate $\det\left(B^{-1} A^T B\right)$, we apply the following properties of determinants for invertible $n \times n$ matrices:

1. **Multiplicative property:** $\det(XYZ) = (\det X)(\det Y)(\det Z)$
2. **Determinant of an inverse:** $\det\left(B^{-1}\right) = \frac{1}{\det B}$
3. **Determinant of a transpose:** $\det\left(A^T\right) = \det A$

---

**2. Step-by-Step Computation**

Applying these properties sequentially:

$$
\begin{aligned}
\det\left(B^{-1} A^T B\right) &= \det\left(B^{-1}\right) \det\left(A^T\right) \det B \\
&= \left(\frac{1}{\det B}\right) (\det A) (\det B) \\
&= \left(\frac{1}{3}\right) (-2) (3) \\
&= -2
\end{aligned}
$$

---

**3. Why the Factors Involving $B$ Cancel**

Because the determinant maps matrices to nonzero real numbers (scalars), multiplication of the individual determinants is commutative:

$$
\left(\frac{1}{\det B}\right) (\det A) (\det B) = \left(\frac{1}{\det B} \cdot \det B\right) \det A = 1 \cdot \det A = \det A
$$

Since $B$ is invertible, $\det B \neq 0$, which guarantees that $\det\left(B^{-1}\right) = \frac{1}{\det B}$ is well-defined and acts as the multiplicative inverse of $\det B$ in $\mathbb{R}$. Consequently, their product equals $1$, leaving only $\det A = -2$.

  


 
