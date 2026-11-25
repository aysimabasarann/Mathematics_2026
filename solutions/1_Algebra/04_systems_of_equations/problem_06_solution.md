### Exercise 6. A System with a Parameter — Which Cases Actually Occur?

Analyze, depending on the parameter $a$, the system

$$
\begin{cases}
x+y=2, \\
ax+ay=4.
\end{cases}
$$

Among the three possibilities — exactly one solution, infinitely many solutions, no solution — determine which actually occur and for which values of $a$. If one type cannot occur, explain why.

---

## Solution

### 1. Setting Up the Augmented Matrix

We write the system as an augmented matrix:

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
a & a & \mid & 4 \\
\end{pmatrix}
$$

To eliminate the entry in the second row, first column, apply the row operation $R_2 \leftarrow R_2 - aR_1$:

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
0 & 0 & \mid & 4 - 2a \\
\end{pmatrix}
$$

### 2. Analysis Based on the Parameter $a$

From the reduced augmented matrix, the second row corresponds to the linear equation:

$$
0x + 0y = 4 - 2a \implies 0 = 4 - 2a
$$

We examine the behavior of the system based on the value of $4 - 2a$:

- **Case 1: When $4 - 2a \neq 0$ (i.e., $a \neq 2$):**
  The equation becomes $0 = 4 - 2a$, where the left-hand side is zero while the right-hand side is nonzero. This creates a contradiction. Therefore, the system has **no solution** for any $a \neq 2$.

- **Case 2: When $4 - 2a = 0$ (i.e., $a = 2$):**
  Substituting $a = 2$ into the augmented matrix gives:

  $$
  \begin{pmatrix}
  1 & 1 & \mid & 2 \\
  0 & 0 & \mid & 0 \\
  \end{pmatrix}
  $$

  The second row becomes $0 = 0$, which is always true and yields no contradiction. The system reduces to a single independent equation:
  
  $$
  x + y = 2
  $$

  Since there are $2$ variables and only $1$ pivot, we have $2 - 1 = 1$ free variable (let $y = t$, where $t \in \mathbb{R}$), giving $x = 2 - t$. Thus, the system has **infinitely many solutions** when $a = 2$.

### 3. Summary of Occurring Cases

Among the three theoretical possibilities:
1. **No solution:** Occurs for all $a \neq 2$.
2. **Infinitely many solutions:** Occurs when $a = 2$.
3. **Exactly one solution:** **Cannot occur** for any value of $a$. 

**Reason why one solution cannot occur:** Geometrically, the two equations represent lines in the plane. The slope of the first line is $-1$, and the slope of the second line is $-\frac{a}{a} = -1$ (when $a \neq 0$) or the equation represents the whole plane/no line if $a=0$. Because the lines are strictly parallel for $a \neq 2$ (different intercepts) and identical for $a = 2$, they never intersect at a single unique point. Algebraically, the coefficient matrix can never have full rank equal to $2$ because the second row is always a multiple of the first row, making the determinant of the coefficient matrix identically zero for all $a$.
