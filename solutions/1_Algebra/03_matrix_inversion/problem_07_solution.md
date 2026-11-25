# Exercise 7. Inverse of a Product

For

$$
A =
\begin{pmatrix}
1 & 1 \\
0 & 1 \\
\end{pmatrix}
$$

and

$$
B =
\begin{pmatrix}
2 & 0 \\
0 & 3 \\
\end{pmatrix}
$$

compute $(AB)^{-1}$ and $B^{-1}A^{-1}$. Check that the results are the same and explain the meaning of the reversed order.

---

## Solution

**1. Computing the Matrices and Their Inverses**

First, we compute the inverses of $A$ and $B$:

$$
A^{-1} =
\begin{pmatrix}
1 & -1 \\
0 & 1 \\
\end{pmatrix}
$$

and

$$
B^{-1} =
\begin{pmatrix}
\frac{1}{2} & 0 \\
0 & \frac{1}{3} \\
\end{pmatrix}
$$

**2. Computing $(AB)^{-1}$**

Next, we compute the product $AB$:

$$
\begin{aligned}
AB &=
\begin{pmatrix}
1 & 1 \\
0 & 1 \\
\end{pmatrix}
\begin{pmatrix}
2 & 0 \\
0 & 3 \\
\end{pmatrix} \\
&=
\begin{pmatrix}
2 & 3 \\
0 & 3 \\
\end{pmatrix}
\end{aligned}
$$

Now, we find the inverse of $AB$:

$$
(AB)^{-1} =
\begin{pmatrix}
\frac{1}{2} & -\frac{1}{2} \\
0 & \frac{1}{3} \\
\end{pmatrix}
$$

**3. Computing $B^{-1}A^{-1}$**

Multiplying $B^{-1}$ and $A^{-1}$:

$$
\begin{aligned}
B^{-1}A^{-1} &=
\begin{pmatrix}
\frac{1}{2} & 0 \\
0 & \frac{1}{3} \\
\end{pmatrix}
\begin{pmatrix}
1 & -1 \\
0 & 1 \\
\end{pmatrix} \\
&=
\begin{pmatrix}
\frac{1}{2} & -\frac{1}{2} \\
0 & \frac{1}{3} \\
\end{pmatrix}
\end{aligned}
$$

Thus, we verify that $(AB)^{-1} = B^{-1}A^{-1}$.

**4. Explanation of the Reversed Order**

When a vector $x$ is multiplied by the product matrix $AB$, the transformation is applied via $(AB)x = A(Bx)$. Here, matrix $B$ acts first on the vector, and matrix $A$ acts second on the resulting vector. To undo this combined operation, we must reverse the sequence of steps: we first undo $A$ by applying $A^{-1}$, and then undo $B$ by applying $B^{-1}$. Therefore, the inverse of the product is given by $(AB)^{-1} = B^{-1}A^{-1}$.



  
