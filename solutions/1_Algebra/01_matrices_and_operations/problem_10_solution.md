Exercise 10. Columns of a Matrix Product

Given

The matrices are

$$
A=
\begin{pmatrix}
1 & 2 & 0 \
0 & 1 & 1 \
\end{pmatrix}
$$

and

$$
B=
\begin{pmatrix}
1 & 2 \
-1 & 0 \
3 & 1 \
\end{pmatrix}
$$

The columns of matrix $B$ are denoted by $b_1$ and $b_2$:

$$
b_1=
\begin{pmatrix}
1 \
-1 \
3 \
\end{pmatrix}
\qquad
b_2=
\begin{pmatrix}
2 \
0 \
1 \
\end{pmatrix}
$$

The required tasks are:

1. Compute $Ab_1$ and $Ab_2$.
2. Compute the matrix product $AB$.
3. Compare the results and explain why the columns of $AB$ are exactly the vectors $Ab_1$ and $Ab_2$.

Solution

1. Computing $Ab_1$ and $Ab_2$

First, multiply matrix $A$ by the first column of $B$:

$$
Ab_1=
\begin{pmatrix}
1 & 2 & 0 \
0 & 1 & 1 \
\end{pmatrix}
\begin{pmatrix}
1 \
-1 \
3 \
\end{pmatrix}
$$

Calculating each entry gives

$$
Ab_1=
\begin{pmatrix}
1(1)+2(-1)+0(3) \
0(1)+1(-1)+1(3) \
\end{pmatrix}

\begin{pmatrix}
-1 \
2 \
\end{pmatrix}
$$

Next, multiply matrix $A$ by the second column of $B$:

$$
Ab_2=
\begin{pmatrix}
1 & 2 & 0 \
0 & 1 & 1 \
\end{pmatrix}
\begin{pmatrix}
2 \
0 \
1 \
\end{pmatrix}
$$

Calculating each entry gives

$$
Ab_2=
\begin{pmatrix}
1(2)+2(0)+0(1) \
0(2)+1(0)+1(1) \
\end{pmatrix}

\begin{pmatrix}
2 \
1 \
\end{pmatrix}
$$

2. Computing the matrix product $AB$

The product $AB$ is defined because the number of columns of $A$ equals the number of rows of $B$.

The resulting matrix has two rows and two columns.

$$
AB=
\begin{pmatrix}
1 & 2 & 0 \
0 & 1 & 1 \
\end{pmatrix}
\begin{pmatrix}
1 & 2 \
-1 & 0 \
3 & 1 \
\end{pmatrix}
$$

Multiplying the corresponding rows and columns gives

$$
AB=
\begin{pmatrix}
1(1)+2(-1)+0(3) & 1(2)+2(0)+0(1) \
0(1)+1(-1)+1(3) & 0(2)+1(0)+1(1) \
\end{pmatrix}
$$

Therefore,

$$
AB=
\begin{pmatrix}
-1 & 2 \
2 & 1 \
\end{pmatrix}
$$

3. Comparing the results

The first column of $AB$ is

$$
\begin{pmatrix}
-1 \
2 \
\end{pmatrix}
=Ab_1
$$

The second column of $AB$ is

$$
\begin{pmatrix}
2 \
1 \
\end{pmatrix}
=Ab_2
$$

Therefore, the matrix product can be written as

$$
AB=
\begin{pmatrix}
Ab_1 & Ab_2
\end{pmatrix}
$$

This happens because matrix multiplication applies matrix $A$ to each column of matrix $B$ separately. Each column of the resulting product is obtained by multiplying $A$ by the corresponding column of $B$.

Conclusion

The calculations confirm that the columns of $AB$ are exactly $Ab_1$ and $Ab_2$. This demonstrates that matrix multiplication can be understood as applying a linear transformation to each column of the second matrix independently.









 
