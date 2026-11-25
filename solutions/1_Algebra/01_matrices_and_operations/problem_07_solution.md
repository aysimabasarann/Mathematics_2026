### Exercise 7. Identity Matrix, Zero Matrix, and Powers

**Problem:**

For

$$
A = \begin{pmatrix}
2 & 1 \\
0 & 2
\end{pmatrix}
$$

compute

$$
AI,\qquad IA,\qquad A+0,\qquad A^2,\qquad A^3.
$$

Explain the roles of the matrices $I$ and $0$, and describe the pattern you observe in successive powers of $A$.

---

## Solution

### 1. Matrix Products with the Identity Matrix ($I$)

For a $2 \times 2$ matrix, the identity matrix is

$$
I = \begin{pmatrix}
1 & 0 \\
0 & 1
\end{pmatrix}
$$

Computing $AI$:

$$
AI = \begin{pmatrix}
2 & 1 \\
0 & 2
\end{pmatrix}
\begin{pmatrix}
1 & 0 \\
0 & 1
\end{pmatrix}
= \begin{pmatrix}
(2)(1) + (1)(0) & (2)(0) + (1)(1) \\
(0)(1) + (2)(0) & (0)(0) + (2)(1)
\end{pmatrix}
= \begin{pmatrix}
2 & 1 \\
0 & 2
\end{pmatrix} = A
$$

Computing $IA$:

$$
IA = \begin{pmatrix}
1 & 0 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
2 & 1 \\
0 & 2
\end{pmatrix}
= \begin{pmatrix}
(1)(2) + (0)(0) & (1)(1) + (0)(2) \\
(0)(2) + (1)(0) & (0)(1) + (1)(2)
\end{pmatrix}
= \begin{pmatrix}
2 & 1 \\
0 & 2
\end{pmatrix} = A
$$

### 2. Matrix Addition with the Zero Matrix ($0$)

For a $2 \times 2$ matrix, the zero matrix is

$$
0 = \begin{pmatrix}
0 & 0 \\
0 & 0
\end{pmatrix}
$$

Computing $A+0$:

$$
A + 0 = \begin{pmatrix}
2 & 1 \\
0 & 2
\end{pmatrix} + \begin{pmatrix}
0 & 0 \\
0 & 0
\end{pmatrix} = \begin{pmatrix}
2+0 & 1+0 \\
0+0 & 2+0
\end{pmatrix} = \begin{pmatrix}
2 & 1 \\
0 & 2
\end{pmatrix} = A
$$

### 3. Computing Successive Powers of $A$

Computing $A^2$:

$$
A^2 = A \cdot A = \begin{pmatrix}
2 & 1 \\
0 & 2
\end{pmatrix}
\begin{pmatrix}
2 & 1 \\
0 & 2
\end{pmatrix}
= \begin{pmatrix}
(2)(2) + (1)(0) & (2)(1) + (1)(2) \\
(0)(2) + (2)(0) & (0)(1) + (2)(2)
\end{pmatrix}
= \begin{pmatrix}
4 & 4 \\
0 & 4
\end{pmatrix}
$$

Computing $A^3$:

$$
A^3 = A^2 \cdot A = \begin{pmatrix}
4 & 4 \\
0 & 4
\end{pmatrix}
\begin{pmatrix}
2 & 1 \\
0 & 2
\end{pmatrix}
= \begin{pmatrix}
(4)(2) + (4)(0) & (4)(1) + (4)(2) \\
(0)(2) + (4)(0) & (0)(1) + (4)(2)
\end{pmatrix}
= \begin{pmatrix}
8 & 12 \\
0 & 8
\end{pmatrix}
$$

### 4. Roles of $I$ and $0$ and Pattern in Powers

* **The Identity Matrix ($I$):** Acts as the multiplicative neutral element. Multiplying any compatible matrix by $I$ leaves the matrix unchanged ($AI = IA = A$).
* **The Zero Matrix ($0$):** Acts as the additive neutral element. Adding the zero matrix to another matrix leaves the matrix unchanged ($A + 0 = A$).
* **Pattern in Successive Powers of $A$:** Observing the computed powers:

$$
A^1 = \begin{pmatrix}
2 & 1 \\
0 & 2
\end{pmatrix}
= \begin{pmatrix}
2^1 & 1 \cdot 2^0 \\
0 & 2^1
\end{pmatrix}
$$

$$
A^2 = \begin{pmatrix}
4 & 4 \\
0 & 4
\end{pmatrix}
= \begin{pmatrix}
2^2 & 2 \cdot 2^1 \\
0 & 2^2
\end{pmatrix}
$$

$$
A^3 = \begin{pmatrix}
8 & 12 \\
0 & 8
\end{pmatrix}
= \begin{pmatrix}
2^3 & 3 \cdot 2^2 \\
0 & 2^3
\end{pmatrix}
$$

In general, for $n \ge 1$, the matrix power $A^n$ follows the pattern:

$$
A^n = \begin{pmatrix}
2^n & n \cdot 2^{n-1} \\
0 & 2^n
\end{pmatrix}
$$

 


 
