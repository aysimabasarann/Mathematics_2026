### Exercise 12. Formula for a Matrix Power

**Problem:**

Let

$$
A = \begin{pmatrix} 1 & 1 \\ 0 & 1 \end{pmatrix}.
$$

Compute $A^2$, $A^3$, and $A^4$, and use them to formulate a conjecture for $A^n$. Then do not stop after checking one more case: assume the formula is true for $n$, multiply by $A$, and explain why you obtain exactly the formula for $n+1$.

---

## Solution

### 1. Computing $A^2$, $A^3$, and $A^4$

First, we compute $A^2$:

$$
A^2 = A \cdot A = \begin{pmatrix} 1 & 1 \\ 0 & 1 \end{pmatrix} \begin{pmatrix} 1 & 1 \\ 0 & 1 \end{pmatrix} = \begin{pmatrix} (1)(1) + (1)(0) & (1)(1) + (1)(1) \\ (0)(1) + (1)(0) & (0)(1) + (1)(1) \end{pmatrix} = \begin{pmatrix} 1 & 2 \\ 0 & 1 \end{pmatrix}
$$

Next, we compute $A^3$:

$$
A^3 = A^2 \cdot A = \begin{pmatrix} 1 & 2 \\ 0 & 1 \end{pmatrix} \begin{pmatrix} 1 & 1 \\ 0 & 1 \end{pmatrix} = \begin{pmatrix} (1)(1) + (2)(0) & (1)(1) + (2)(1) \\ (0)(1) + (1)(0) & (0)(1) + (1)(1) \end{pmatrix} = \begin{pmatrix} 1 & 3 \\ 0 & 1 \end{pmatrix}
$$

Then, we compute $A^4$:

$$
A^4 = A^3 \cdot A = \begin{pmatrix} 1 & 3 \\ 0 & 1 \end{pmatrix} \begin{pmatrix} 1 & 1 \\ 0 & 1 \end{pmatrix} = \begin{pmatrix} (1)(1) + (3)(0) & (1)(1) + (3)(1) \\ (0)(1) + (1)(0) & (0)(1) + (1)(1) \end{pmatrix} = \begin{pmatrix} 1 & 4 \\ 0 & 1 \end{pmatrix}
$$

### 2. Conjecture for $A^n$

Observing the computed powers:
* For $n = 1$, the top-right entry is $1$.
* For $n = 2$, the top-right entry is $2$.
* For $n = 3$, the top-right entry is $3$.
* For $n = 4$, the top-right entry is $4$.

Meanwhile, the diagonal entries remain $1$ and the bottom-left entry remains $0$. Based on this pattern, we conjecture that for any positive integer $n \ge 1$:

$$
A^n = \begin{pmatrix} 1 & n \\ 0 & 1 \end{pmatrix}
$$

### 3. Proof by Mathematical Induction (From $n$ to $n+1$)

**Base Case ($n = 1$):**

$$
A^1 = \begin{pmatrix} 1 & 1 \\ 0 & 1 \end{pmatrix}
$$

The formula holds for $n = 1$.

**Inductive Step:**
Assume the conjecture holds for an arbitrary positive integer $n$, meaning that:

$$
A^n = \begin{pmatrix} 1 & n \\ 0 & 1 \end{pmatrix}
$$

To find $A^{n+1}$, we multiply our assumed expression for $A^n$ by $A$:

$$
A^{n+1} = A^n \cdot A = \begin{pmatrix} 1 & n \\ 0 & 1 \end{pmatrix} \begin{pmatrix} 1 & 1 \\ 0 & 1 \end{pmatrix} = \begin{pmatrix} (1)(1) + (n)(0) & (1)(1) + (n)(1) \\ (0)(1) + (1)(0) & (0)(1) + (1)(1) \end{pmatrix} = \begin{pmatrix} 1 & n + 1 \\ 0 & 1 \end{pmatrix}
$$

**Explanation:**
When multiplying $A^n$ by $A$, the top-left entry remains $1 \cdot 1 + n \cdot 0 = 1$, the bottom-left entry remains $0 \cdot 1 + 1 \cdot 0 = 0$, and the bottom-right entry remains $0 \cdot 1 + 1 \cdot 1 = 1$. In the top-right entry, taking the dot product of the first row of $A^n$ ($\begin{pmatrix} 1 & n \end{pmatrix}$) with the second column of $A$ ($\begin{pmatrix} 1 \\ 1 \end{pmatrix}$) adds $1$ to $n$, yielding $n + 1$.

This is precisely the conjectured formula evaluated at $n + 1$. By the principle of mathematical induction, the formula $A^n = \begin{pmatrix} 1 & n \\ 0 & 1 \end{pmatrix}$ holds for all integers $n \ge 1$.

