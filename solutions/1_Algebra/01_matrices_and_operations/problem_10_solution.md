## Question

Given the matrices

$$
A =
\begin{pmatrix}
1 & 2 & 0 \\
0 & 1 & 1 \\
\end{pmatrix}
$$

and

$$
B =
\begin{pmatrix}
1 & 2 \\
-1 & 0 \\
3 & 1 \\
\end{pmatrix}
$$

denote the columns of $B$ by $b_1$ and $b_2$.

1. Compute $Ab_1$ and $Ab_2$.
2. Compute the matrix $AB$.
3. Compare the results and explain why the columns of $AB$ are exactly the vectors $Ab_1$ and $Ab_2$.

---

## Solution

The columns of the $3 \times 2$ matrix $B$ are

$$
b_1 =
\begin{pmatrix}
1 \\
-1 \\
3 \\
\end{pmatrix}
$$

and

$$
b_2 =
\begin{pmatrix}
2 \\
0 \\
1 \\
\end{pmatrix}
$$

### 1. Compute $Ab_1$ and $Ab_2$

To compute $Ab_1$, multiply the $2 \times 3$ matrix $A$ by the $3 \times 1$ column vector $b_1$:

$$
\begin{aligned}
Ab_1 &=
\begin{pmatrix}
1 & 2 & 0 \\
0 & 1 & 1 \\
\end{pmatrix}
\begin{pmatrix}
1 \\
-1 \\
3 \\
\end{pmatrix} \\
&=
\begin{pmatrix}
1 \cdot 1 + 2 \cdot (-1) + 0 \cdot 3 \\
0 \cdot 1 + 1 \cdot (-1) + 1 \cdot 3 \\
\end{pmatrix} \\
&=
\begin{pmatrix}
1 - 2 + 0 \\
0 - 1 + 3 \\
\end{pmatrix} \\
&=
\begin{pmatrix}
-1 \\
2 \\
\end{pmatrix}
\end{aligned}
$$

Similarly, to compute $Ab_2$, multiply the matrix $A$ by the second column vector $b_2$:

$$
\begin{aligned}
Ab_2 &=
\begin{pmatrix}
1 & 2 & 0 \\
0 & 1 & 1 \\
\end{pmatrix}
\begin{pmatrix}
2 \\
0 \\
1 \\
\end{pmatrix} \\
&=
\begin{pmatrix}
1 \cdot 2 + 2 \cdot 0 + 0 \cdot 1 \\
0 \cdot 2 + 1 \cdot 0 + 1 \cdot 1 \\
\end{pmatrix} \\
&=
\begin{pmatrix}
2 + 0 + 0 \\
0 + 0 + 1 \\
\end{pmatrix} \\
&=
\begin{pmatrix}
2 \\
1 \\
\end{pmatrix}
\end{aligned}
$$

### 2. Compute the matrix $AB$

Since $A$ has dimensions $2 \times 3$ and $B$ has dimensions $3 \times 2$, the product $AB$ is a $2 \times 2$ matrix whose $(i,j)$-entry is the dot product of row $i$ of $A$ and column $j$ of $B$:

$$
\begin{aligned}
AB &=
\begin{pmatrix}
1 & 2 & 0 \\
0 & 1 & 1 \\
\end{pmatrix}
\begin{pmatrix}
1 & 2 \\
-1 & 0 \\
3 & 1 \\
\end{pmatrix} \\
&=
\begin{pmatrix}
1 \cdot 1 + 2 \cdot (-1) + 0 \cdot 3 & 1 \cdot 2 + 2 \cdot 0 + 0 \cdot 1 \\
0 \cdot 1 + 1 \cdot (-1) + 1 \cdot 3 & 0 \cdot 2 + 1 \cdot 0 + 1 \cdot 1 \\
\end{pmatrix} \\
&=
\begin{pmatrix}
-1 & 2 \\
2 & 1 \\
\end{pmatrix}
\end{aligned}
$$

### 3. Comparison and explanation

Comparing the matrix $AB$ with the vectors $Ab_1$ and $Ab_2$ shows that its columns are precisely $Ab_1$ and $Ab_2$:

$$
AB =
\begin{pmatrix}
-1 & 2 \\
2 & 1 \\
\end{pmatrix}
$$

By definition of matrix multiplication, the $j$-th column of $AB$ is formed exclusively by taking the dot products of each row of $A$ with the $j$-th column of $B$. Because no other columns of $B$ participate in computing the $j$-th column of $AB$, that column is identical to the matrix-vector product $Ab_j$.
    
