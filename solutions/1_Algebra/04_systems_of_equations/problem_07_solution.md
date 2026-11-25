### Exercise 7. Choosing a Method Deliberately

Do not solve all of the following systems completely. For each situation, choose the method that best uses its structure and justify your choice:

1. one system with a triangular coefficient matrix

$$
\begin{cases}
2x-y=3, \\
4y=8;
\end{cases}
$$

2. three systems $Ax=b_i$ with the same invertible matrix $A$, when $A^{-1}$ is already known;
3. one $3\times3$ system for which the inverse matrix is not given and the goal is only to find one solution vector.

For case 1, carry out the chosen method completely. For cases 2 and 3, describe the plan and indicate which part of the computation would be reusable or unnecessary. Do not judge a method by its name alone — refer to the number of right-hand sides and the structure of the matrix.

---

## Solution

### 1. Triangular Coefficient Matrix

**Chosen Method:** Direct **back-substitution**.

**Justification:** The coefficient matrix is already in upper triangular form, meaning no row operations or forward elimination steps are required. Furthermore, there is only a single right-hand side vector, making matrix inversion completely unnecessary.

**Complete Solution:**

From the second equation, solve directly for $y$:

$$
4y = 8 \implies y = 2
$$

Substitute $y = 2$ into the first equation to solve for $x$:

$$
2x - 2 = 3 \implies 2x = 5 \implies x = \frac{5}{2}
$$

Thus, the unique solution is $(x, y) = \left(\frac{5}{2}, 2\right)$.

### 2. Three Systems $Ax = b_i$ with the Same Matrix $A$ and Known $A^{-1}$

**Chosen Method:** Direct matrix-vector multiplication using the known inverse:

$$
x_i = A^{-1}b_i \quad (i = 1, 2, 3)
$$

**Plan and Computational Efficiency:**

- **Reusable part:** Because the coefficient matrix $A$ is shared across all three systems and $A^{-1}$ is already computed and available, this same inverse matrix $A^{-1}$ is directly reused for each of the three right-hand side vectors $b_1, b_2, b_3$.
- **Unnecessary part:** Performing Gaussian elimination three separate times or recomputing $A^{-1}$ from scratch is completely unnecessary. Computing the solution vectors reduces strictly to three matrix-vector multiplications ($A^{-1}b_1$, $A^{-1}b_2$, and $A^{-1}b_3$).

### 3. Single $3 \times 3$ System Without a Known Inverse

**Chosen Method:** **Gaussian elimination** with back-substitution.

**Plan and Computational Efficiency:**

- **Plan:** Form the $3 \times 4$ augmented matrix $[A \mid b]$, apply elementary row operations to reduce the coefficient part to row echelon form, and find the single solution vector via back-substitution.
- **Unnecessary part:** Computing the full inverse matrix $A^{-1}$ (e.g., via Gauss-Jordan elimination on $[A \mid I]$ or using determinants and cofactors) is unnecessary. Because there is only one right-hand side vector $b$, finding $A^{-1}$ requires substantially more arithmetic operations than reducing a single augmented column.
- **Reusable part:** Since there is only one right-hand side and no subsequent systems to solve, no reusable inverse operator needs to be stored for later computations.
