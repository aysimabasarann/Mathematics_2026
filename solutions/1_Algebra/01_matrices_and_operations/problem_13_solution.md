### Exercise 13. A Recurrence Written in Matrix Form

**Problem:**

Let

$$
F = \begin{pmatrix} 1 & 1 \\ 1 & 0 \end{pmatrix}.
$$

Compute $F^2$, $F^3$, $F^4$, and $F^5$. Compare the numbers obtained with the sequence

$$
0, 1, 1, 2, 3, 5, 8, \ldots
$$

and describe the relationship you observe. Then compute

$$
F \begin{pmatrix} a \\ b \end{pmatrix}
$$

and explain how this multiplication performs one recurrence step: it creates the sum of two consecutive terms and keeps one of them for the next step.

---

## Solution

### 1. Computing Successive Powers of $F$

First, we compute $F^2$:

$$
F^2 = \begin{pmatrix} 1 & 1 \\ 1 & 0 \end{pmatrix} \begin{pmatrix} 1 & 1 \\ 1 & 0 \end{pmatrix} = \begin{pmatrix} (1)(1) + (1)(1) & (1)(1) + (1)(0) \\ (1)(1) + (0)(1) & (1)(1) + (0)(0) \end{pmatrix} = \begin{pmatrix} 2 & 1 \\ 1 & 1 \end{pmatrix}
$$

Next, we compute $F^3$:

$$
F^3 = F^2 \cdot F = \begin{pmatrix} 2 & 1 \\ 1 & 1 \end{pmatrix} \begin{pmatrix} 1 & 1 \\ 1 & 0 \end{pmatrix} = \begin{pmatrix} (2)(1) + (1)(1) & (2)(1) + (1)(0) \\ (1)(1) + (1)(1) & (1)(1) + (1)(0) \end{pmatrix} = \begin{pmatrix} 3 & 2 \\ 2 & 1 \end{pmatrix}
$$

Then, we compute $F^4$:

$$
F^4 = F^3 \cdot F = \begin{pmatrix} 3 & 2 \\ 2 & 1 \end{pmatrix} \begin{pmatrix} 1 & 1 \\ 1 & 0 \end{pmatrix} = \begin{pmatrix} (3)(1) + (2)(1) & (3)(1) + (2)(0) \\ (2)(1) + (1)(1) & (2)(1) + (1)(0) \end{pmatrix} = \begin{pmatrix} 5 & 3 \\ 3 & 2 \end{pmatrix}
$$

Finally, we compute $F^5$:

$$
F^5 = F^4 \cdot F = \begin{pmatrix} 5 & 3 \\ 3 & 2 \end{pmatrix} \begin{pmatrix} 1 & 1 \\ 1 & 0 \end{pmatrix} = \begin{pmatrix} (5)(1) + (3)(1) & (5)(1) + (3)(0) \\ (3)(1) + (2)(1) & (3)(1) + (2)(0) \end{pmatrix} = \begin{pmatrix} 8 & 5 \\ 5 & 3 \end{pmatrix}
$$

### 2. Comparison with the Fibonacci Sequence

The given sequence $0, 1, 1, 2, 3, 5, 8, \ldots$ is the well-known Fibonacci sequence, where each term is the sum of the two preceding ones. 

Comparing this sequence with the entries of our computed matrix powers:
* $F^2 = \begin{pmatrix} 2 & 1 \\ 1 & 1 \end{pmatrix}$ contains Fibonacci numbers $F_3 = 2$, $F_2 = 1$, $F_1 = 1$.
* $F^3 = \begin{pmatrix} 3 & 2 \\ 2 & 1 \end{pmatrix}$ contains $F_4 = 3$, $F_3 = 2$, $F_2 = 1$.
* $F^4 = \begin{pmatrix} 5 & 3 \\ 3 & 2 \end{pmatrix}$ contains $F_5 = 5$, $F_4 = 3$, $F_3 = 2$.
* $F^5 = \begin{pmatrix} 8 & 5 \\ 5 & 3 \end{pmatrix}$ contains $F_6 = 8$, $F_5 = 5$, $F_4 = 3$, $F_3 = 2$.

In general, for any integer $n \ge 1$, the matrix power $F^n$ has the structure:

$$
F^n = \begin{pmatrix} F_{n+1} & F_n \\ F_n & F_{n-1} \end{pmatrix}
$$

### 3. Matrix Multiplication as a Recurrence Step

Computing the product of $F$ with an arbitrary vector containing two consecutive terms $\begin{pmatrix} a \\ b \end{pmatrix}$:

$$
F \begin{pmatrix} a \\ b \end{pmatrix} = \begin{pmatrix} 1 & 1 \\ 1 & 0 \end{pmatrix} \begin{pmatrix} a \\ b \end{pmatrix} = \begin{pmatrix} (1)(a) + (1)(b) \\ (1)(a) + (0)(b) \end{pmatrix} = \begin{pmatrix} a + b \\ a \end{pmatrix}
$$

**Explanation:**
This operation performs one complete step of a numerical recurrence:
1. The top entry becomes $a + b$, which is the sum of the two current consecutive terms, generating the next term in the sequence.
2. The bottom entry becomes $a$, which shifts the previous top term down to serve as the older term in the subsequent step. 

Repeated multiplication by $F$ thus advances the recurrence relation efficiently.

