 ### Exercise 15. Comparing Methods

For

$$
A=
\begin{pmatrix}
2 & 4 & 2 \\
1 & 3 & 0 \\
0 & 2 & 5 \\
\end{pmatrix}
$$

compute $\det A$ by two methods:
1. by Sarrus' rule,
2. by simplifying the matrix first with row operations.

Compare the amount of computation and explain when row operations are more advantageous.

---

## Solution

### 1. Method 1: Computing $\det A$ Using Sarrus' Rule

To apply Sarrus' rule, we repeat the first two columns of $A$ to the right of the matrix:

$$
\begin{pmatrix}
2 & 4 & 2 & \mid & 2 & 4 \\
1 & 3 & 0 & \mid & 1 & 3 \\
0 & 2 & 5 & \mid & 0 & 2 \\
\end{pmatrix}
$$

First, we compute the sum of the products along the three main diagonals (top-left to bottom-right):

$$
D_1 = (2)(3)(5) + (4)(0)(0) + (2)(1)(2) = 30 + 0 + 4 = 34
$$

Next, we compute the sum of the products along the three anti-diagonals (bottom-left to top-right):

$$
D_2 = (0)(3)(2) + (2)(0)(2) + (5)(1)(4) = 0 + 0 + 20 = 20
$$

Subtracting $D_2$ from $D_1$ gives:

$$
\det A = D_1 - D_2 = 34 - 20 = 14
$$

### 2. Method 2: Simplifying First with Row Operations

We reduce $A$ to upper-triangular form while tracking the effect of each operation on the determinant.

**Step 1:** Factor out $2$ from the first row ($R_1 \leftarrow \frac{1}{2}R_1$). Factoring a scalar $k = 2$ out of a single row multiplies the determinant by $2$:

$$
\det A = 2 \det
\begin{pmatrix}
1 & 2 & 1 \\
1 & 3 & 0 \\
0 & 2 & 5 \\
\end{pmatrix}
$$

**Step 2:** Eliminate the entry below the pivot in the first column by applying $R_2 \leftarrow R_2 - R_1$. Adding a multiple of one row to another does not change the determinant:

$$
\det A = 2 \det
\begin{pmatrix}
1 & 2 & 1 \\
0 & 1 & -1 \\
0 & 2 & 5 \\
\end{pmatrix}
$$

**Step 3:** Eliminate the entry below the pivot in the second column by applying $R_3 \leftarrow R_3 - 2R_2$. This also leaves the determinant unchanged:

$$
\det A = 2 \det
\begin{pmatrix}
1 & 2 & 1 \\
0 & 1 & -1 \\
0 & 0 & 7 \\
\end{pmatrix}
$$

Now, multiplying the main diagonal entries of the upper-triangular matrix gives:

$$
\det A = 2 \cdot (1)(1)(7) = 14
$$

Both methods yield $\det A = 14$.

### 3. Comparison of Methods

* **Computational Effort:** For a $3 \times 3$ matrix—especially one that already contains zeros like $a_{23} = 0$ and $a_{31} = 0$—Sarrus' rule requires very few multiplications ($6$ triple products, half of which vanish) and is extremely fast. Row operations require several matrix rewrites and careful tracking of scaling factors.
* **When Row Operations Are More Advantageous:** Row reduction becomes significantly more advantageous for matrices of size $4 \times 4$ and larger, where Sarrus' rule does not apply at all and cofactor expansion grows factorially at $O(n!)$ complexity. Row operations reduce the computational cost to polynomial time of $O(n^3)$, making them the standard method for large matrices, matrices with common row factors, or matrices containing symbolic parameters.


 
