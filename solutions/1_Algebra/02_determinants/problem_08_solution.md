### Exercise 8. Determinant of a Product

Let $A,B$ be square matrices such that $\det A=3$ and $\det B=-5$. Compute $\det(AB)$, $\det(BA)$ and, if it exists, $\det(A^{-1}B)$. Explain why the first two results are equal even though usually $AB\neq BA$.

---

## Solution

Given two square matrices $A$ and $B$ of the same size with $\det A = 3$ and $\det B = -5$, we compute each determinant using the multiplicative properties of determinants.

### 1. Computing $\det(AB)$

**Property:** The determinant of a product of two square matrices of the same order equals the product of their individual determinants:

$$
\det(AB) = (\det A)(\det B)
$$

Substituting the given values:

$$
\det(AB) = (3)(-5) = -15
$$

### 2. Computing $\det(BA)$

Using the same multiplicative property in reverse order:

$$
\det(BA) = (\det B)(\det A)
$$

Substituting the given values:

$$
\det(BA) = (-5)(3) = -15
$$

### 3. Computing $\det(A^{-1}B)$

First, we check whether $A^{-1}$ exists. Since $\det A = 3 \neq 0$, the matrix $A$ is invertible, so $A^{-1}$ exists.

**Property:** For an invertible matrix $A$, the determinant of its inverse is the reciprocal of its determinant:

$$
\det(A^{-1}) = \frac{1}{\det A} = \frac{1}{3}
$$

Now, applying the product property of determinants to $A^{-1}B$:

$$
\det(A^{-1}B) = \det(A^{-1})\det(B) = \left(\frac{1}{3}\right)(-5) = -\frac{5}{3}
$$

### 4. Explanation of Why $\det(AB) = \det(BA)$

Although matrix multiplication is generally non-commutative ($AB \neq BA$), the determinants $\det A$ and $\det B$ are ordinary real numbers (scalars). Multiplication of real numbers is commutative, meaning:

$$
(\det A)(\det B) = (\det B)(\det A)
$$

Consequently, $\det(AB)$ and $\det(BA)$ always yield the exact same scalar value, even when the product matrices $AB$ and $BA$ themselves are different.

