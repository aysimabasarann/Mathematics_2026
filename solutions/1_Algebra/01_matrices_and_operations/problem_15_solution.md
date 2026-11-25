### Exercise 15. Associativity of Multiplication and Different Calculation Paths

**Problem:**

Given

$$
A = \begin{pmatrix} 1 & 2 & 0 \\ 0 & 1 & 1 \end{pmatrix},\quad B = \begin{pmatrix} 1 & 0 \\ 2 & 1 \\ -1 & 3 \end{pmatrix},\quad C = \begin{pmatrix} 2 & 1 \\ 0 & -1 \end{pmatrix}.
$$

Compute $(AB)C$ and $A(BC)$. Compare the results and the number of intermediate operations. Explain what associativity of matrix multiplication means in this example.

---

## Solution

### 1. Computing $(AB)C$ (Path 1)

First, we compute the product $AB$:
* Matrix $A$ is $2 \times 3$ and matrix $B$ is $3 \times 2$, so $AB$ is a $2 \times 2$ matrix.

$$
AB = \begin{pmatrix} 1 & 2 & 0 \\ 0 & 1 & 1 \end{pmatrix} \begin{pmatrix} 1 & 0 \\ 2 & 1 \\ -1 & 3 \end{pmatrix} = \begin{pmatrix} (1)(1) + (2)(2) + (0)(-1) & (1)(0) + (2)(1) + (0)(3) \\ (0)(1) + (1)(2) + (1)(-1) & (0)(0) + (1)(1) + (1)(3) \end{pmatrix} = \begin{pmatrix} 5 & 2 \\ 1 & 4 \end{pmatrix}
$$

Next, we multiply the resulting matrix $AB$ by $C$:
* $AB$ is $2 \times 2$ and $C$ is $2 \times 2$, so $(AB)C$ is a $2 \times 2$ matrix.

$$
(AB)C = \begin{pmatrix} 5 & 2 \\ 1 & 4 \end{pmatrix} \begin{pmatrix} 2 & 1 \\ 0 & -1 \end{pmatrix} = \begin{pmatrix} (5)(2) + (2)(0) & (5)(1) + (2)(-1) \\ (1)(2) + (4)(0) & (1)(1) + (4)(-1) \end{pmatrix} = \begin{pmatrix} 10 & 3 \\ 2 & -3 \end{pmatrix}
$$

### 2. Computing $A(BC)$ (Path 2)

First, we compute the product $BC$:
* Matrix $B$ is $3 \times 2$ and matrix $C$ is $2 \times 2$, so $BC$ is a $3 \times 2$ matrix.

$$
BC = \begin{pmatrix} 1 & 0 \\ 2 & 1 \\ -1 & 3 \end{pmatrix} \begin{pmatrix} 2 & 1 \\ 0 & -1 \end{pmatrix} = \begin{pmatrix} (1)(2) + (0)(0) & (1)(1) + (0)(-1) \\ (2)(2) + (1)(0) & (2)(1) + (1)(-1) \\ (-1)(2) + (3)(0) & (-1)(1) + (3)(-1) \end{pmatrix} = \begin{pmatrix} 2 & 1 \\ 4 & 1 \\ -2 & -4 \end{pmatrix}
$$

Next, we multiply matrix $A$ by the resulting matrix $BC$:
* Matrix $A$ is $2 \times 3$ and $BC$ is $3 \times 2$, so $A(BC)$ is a $2 \times 2$ matrix.

$$
A(BC) = \begin{pmatrix} 1 & 2 & 0 \\ 0 & 1 & 1 \end{pmatrix} \begin{pmatrix} 2 & 1 \\ 4 & 1 \\ -2 & -4 \end{pmatrix} = \begin{pmatrix} (1)(2) + (2)(4) + (0)(-2) & (1)(1) + (2)(1) + (0)(-4) \\ (0)(2) + (1)(4) + (1)(-2) & (0)(1) + (1)(1) + (1)(-4) \end{pmatrix}
$$

Simplifying each entry:

$$
A(BC) = \begin{pmatrix} 2 + 8 + 0 & 1 + 2 + 0 \\ 0 + 4 - 2 & 0 + 1 - 4 \end{pmatrix} = \begin{pmatrix} 10 & 3 \\ 2 & -3 \end{pmatrix}
$$

### 3. Comparison and Operation Count

Comparing the results:

$$
(AB)C = \begin{pmatrix} 10 & 3 \\ 2 & -3 \end{pmatrix} = A(BC)
$$

**Operation Count Analysis:**
* **Path 1 ($(AB)C$):** 
  - $AB$ requires multiplying a $(2 \times 3)$ by a $(3 \times 2)$ matrix, which takes $2 \times 2 \times 3 = 12$ scalar multiplications.
  - $(AB)C$ requires multiplying a $(2 \times 2)$ by a $(2 \times 2)$ matrix, which takes $2 \times 2 \times 2 = 8$ scalar multiplications.
  - Total for Path 1: $12 + 8 = 20$ scalar multiplications.
* **Path 2 ($A(BC)$):**
  - $BC$ requires multiplying a $(3 \times 2)$ by a $(2 \times 2)$ matrix, which takes $3 \times 2 \times 2 = 12$ scalar multiplications.
  - $A(BC)$ requires multiplying a $(2 \times 3)$ by a $(3 \times 2)$ matrix, which takes $2 \times 2 \times 3 = 12$ scalar multiplications.
  - Total for Path 2: $12 + 12 = 24$ scalar multiplications.

### 4. Meaning of Associativity

**Explanation:**
The property of associativity states that the grouping of matrices in a product does not change the final resulting matrix ($ \left(AB\right)C = A\left(BC\right) $). 

Although both calculation paths yield the exact same final matrix, the number of intermediate arithmetic operations can differ depending on the dimensions of the matrices involved. In practical applications (such as computer graphics and numerical linear algebra), choosing the more efficient grouping path minimizes computational cost.
