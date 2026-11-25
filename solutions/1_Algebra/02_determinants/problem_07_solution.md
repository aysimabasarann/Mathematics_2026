### Exercise 7. Using Properties Instead of Recomputing

Suppose that for a $3\times3$ matrix, $\det A=-4$. Compute

$$
\det(2A),\qquad \det(A^T),\qquad \det(A^2),\qquad \det(-A).
$$

Justify each answer using the appropriate property.

---

## Solution

Given that $A$ is a $3 \times 3$ matrix (so its order is $n = 3$) and $\det A = -4$, we compute each determinant using fundamental determinant properties.

### 1. Computing $\det(2A)$

**Property:** Multiplying an $n \times n$ matrix $A$ by a scalar $k$ multiplies its determinant by $k^n$:

$$
\det(kA) = k^n \det A
$$

Applying this property with $k = 2$ and $n = 3$:

$$
\det(2A) = 2^3 \det A = 8 \cdot (-4) = -32
$$

### 2. Computing $\det(A^T)$

**Property:** Transposing a square matrix does not change its determinant:

$$
\det(A^T) = \det A
$$

Applying this property:

$$
\det(A^T) = -4
$$

### 3. Computing $\det(A^2)$

**Property:** The determinant of a product of two square matrices of the same size is the product of their determinants ($\det(AB) = \det A \cdot \det B$). In particular, for a matrix power $A^m$, $\det(A^m) = (\det A)^m$.

Applying this property for $m = 2$:

$$
\det(A^2) = (\det A)^2 = (-4)^2 = 16
$$

### 4. Computing $\det(-A)$

**Property:** Since $-A = (-1)A$, we apply the scalar multiplication property $\det(kA) = k^n \det A$ with $k = -1$ and $n = 3$:

$$
\det(-A) = (-1)^3 \det A = (-1) \cdot (-4) = 4
$$

