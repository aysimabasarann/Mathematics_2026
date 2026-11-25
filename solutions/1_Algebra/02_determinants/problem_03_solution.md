### Exercise 3. Swapping Two Rows

For

$$
A=
\begin{pmatrix}
1 & 2 & 0 \\
0 & 3 & 1 \\
2 & 1 & 1 \\
\end{pmatrix}
$$

compute $\det A$. Then form a matrix $B$ by swapping the first and second rows of $A$.

First predict $\det B$ using a determinant property, and then verify your prediction by calculation.

---

## Solution

### 1. Computing $\det A$

To compute the determinant of $A$, we can expand along the first row or use Sarrus' rule. Using Sarrus' rule:

$$
\det A = 1 \cdot \det\begin{pmatrix} 3 & 1 \\ 1 & 1 \end{pmatrix} - 2 \cdot \det\begin{pmatrix} 0 & 1 \\ 2 & 1 \end{pmatrix} + 0 \cdot \det\begin{pmatrix} 0 & 3 \\ 2 & 1 \end{pmatrix}
$$

Evaluating the $2 \times 2$ determinants:

$$
\det A = 1(3 \cdot 1 - 1 \cdot 1) - 2(0 \cdot 1 - 1 \cdot 2) + 0 = 1(2) - 2(-2) = 2 + 4 = 6
$$

Thus, $\det A = 6$.

### 2. Predicting $\det B$ Using Determinant Properties

By definition, the matrix $B$ is formed by swapping the first and second rows of $A$. 

A fundamental property of determinants states that **swapping any two rows of a matrix multiplies the determinant by $-1$**. Therefore, we predict that:

$$
\det B = -\det A = -6
$$

### 3. Verifying the Prediction by Direct Calculation

First, we construct matrix $B$ by swapping rows $R_1$ and $R_2$ of $A$:

$$
B =
\begin{pmatrix}
0 & 3 & 1 \\
1 & 2 & 0 \\
2 & 1 & 1 \\
\end{pmatrix}
$$

Next, we compute $\det B$ by expanding along the first row:

$$
\det B = 0 \cdot \det\begin{pmatrix} 2 & 0 \\ 1 & 1 \end{pmatrix} - 3 \cdot \det\begin{pmatrix} 1 & 0 \\ 2 & 1 \end{pmatrix} + 1 \cdot \det\begin{pmatrix} 1 & 2 \\ 2 & 1 \end{pmatrix}
$$

Evaluating each term:

$$
\det B = 0 - 3(1 \cdot 1 - 0 \cdot 2) + 1(1 \cdot 1 - 2 \cdot 2) = -3(1) + 1(-3) = -3 - 3 = -6
$$

The direct calculation yields $\det B = -6$, which perfectly matches our theoretical prediction.

 

 
