# Exercise 10. Matrix Multiplication and Column Vectors

Let

$$
A =
\begin{pmatrix}
1 & 2 \\
3 & 4 \\
\end{pmatrix}
$$

and

$$
B =
\begin{pmatrix}
5 & 6 \\
7 & 8 \\
\end{pmatrix}
$$

Let $b_1$ and $b_2$ denote the first and second columns of $B$, respectively.

1. Compute $Ab_1$ and $Ab_2$.
2. Compute the matrix product $AB$.
3. Explain why the resulting vectors from part (1) are precisely the columns of $AB$.

---

## Solution

**1. Computing $Ab_1$ and $Ab_2$**

The columns of $B$ are

$$
b_1 =
\begin{pmatrix}
5 \\
7 \\
\end{pmatrix}
$$

and

$$
b_2 =
\begin{pmatrix}
6 \\
8 \\
\end{pmatrix}
$$

Multiplying $A$ by $b_1$:

$$
\begin{aligned}
Ab_1 &=
\begin{pmatrix}
1 & 2 \\
3 & 4 \\
\end{pmatrix}
\begin{pmatrix}
5 \\
7 \\
\end{pmatrix} \\
&=
\begin{pmatrix}
1(5) + 2(7) \\
3(5) + 4(7) \\
\end{pmatrix} \\
&=
\begin{pmatrix}
19 \\
43 \\
\end{pmatrix}
\end{aligned}
$$

Multiplying $A$ by $b_2$:

$$
\begin{aligned}
Ab_2 &=
\begin{pmatrix}
1 & 2 \\
3 & 4 \\
\end{pmatrix}
\begin{pmatrix}
6 \\
8 \\
\end{pmatrix} \\
&=
\begin{pmatrix}
1(6) + 2(8) \\
3(6) + 4(8) \\
\end{pmatrix} \\
&=
\begin{pmatrix}
22 \\
50 \\
\end{pmatrix}
\end{aligned}
$$

**2. Computing the Product $AB$**

Using standard matrix multiplication:

$$
\begin{aligned}
AB &=
\begin{pmatrix}
1 & 2 \\
3 & 4 \\
\end{pmatrix}
\begin{pmatrix}
5 & 6 \\
7 & 8 \\
\end{pmatrix} \\
&=
\begin{pmatrix}
1(5) + 2(7) & 1(6) + 2(8) \\
3(5) + 4(7) & 3(6) + 4(8) \\
\end{pmatrix} \\
&=
\begin{pmatrix}
19 & 22 \\
43 & 50 \\
\end{pmatrix}
\end{aligned}
$$

**3. Explanation**

By definition of matrix multiplication, if $B$ has columns $b_1$ and $b_2$, the product $AB$ is formed by multiplying $A$ with each column of $B$ individually:

$$
AB = A \begin{pmatrix} b_1 & b_2 \end{pmatrix} = \begin{pmatrix} Ab_1 & Ab_2 \end{pmatrix}
$$

Therefore, the columns of $AB$ are precisely the vectors $Ab_1$ and $Ab_2$ computed in the first part.








 
