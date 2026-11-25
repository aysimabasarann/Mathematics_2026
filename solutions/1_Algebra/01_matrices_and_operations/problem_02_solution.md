### Exercise 2. Addition and Scalar Multiplication

**Problem:**

For

$$
A = \begin{pmatrix}
1 & 2 \\
-1 & 3
\end{pmatrix}
$$

and

$$
B = \begin{pmatrix}
4 & -2 \\
0 & 5
\end{pmatrix}
$$

compute

$$
A+B,\qquad A-B,\qquad 3A-2B.
$$

Explain why matrix addition is possible only for matrices of the same size.

---

## Solution

### 1. Matrix Addition ($A+B$)

Matrix addition is performed entry by entry:

$$
A + B = \begin{pmatrix}
1 + 4 & 2 + (-2) \\
-1 + 0 & 3 + 5
\end{pmatrix} = \begin{pmatrix}
5 & 0 \\
-1 & 8
\end{pmatrix}
$$

### 2. Matrix Subtraction ($A-B$)

Matrix subtraction is similarly performed entry by entry:

$$
A - B = \begin{pmatrix}
1 - 4 & 2 - (-2) \\
-1 - 0 & 3 - 5
\end{pmatrix} = \begin{pmatrix}
-3 & 4 \\
-1 & -2
\end{pmatrix}
$$

### 3. Scalar Multiplication and Combination ($3A-2B$)

First, multiply each entry of $A$ by $3$ and each entry of $B$ by $2$:

$$
3A = \begin{pmatrix}
3(1) & 3(2) \\
3(-1) & 3(3)
\end{pmatrix} = \begin{pmatrix}
3 & 6 \\
-3 & 9
\end{pmatrix}
$$

$$
2B = \begin{pmatrix}
2(4) & 2(-2) \\
2(0) & 2(5)
\end{pmatrix} = \begin{pmatrix}
8 & -4 \\
0 & 10
\end{pmatrix}
$$

Then, subtract the resulting matrices:

$$
3A - 2B = \begin{pmatrix}
3 - 8 & 6 - (-4) \\
-3 - 0 & 9 - 10
\end{pmatrix} = \begin{pmatrix}
-5 & 10 \\
-3 & -1
\end{pmatrix}
$$

### 4. Dimensional Compatibility for Addition

Matrix addition and subtraction are defined only for matrices of the same size (dimensions) because the operations are carried out entry by entry. If the dimensions differed, there would be no corresponding entry in the second matrix for some elements in the first matrix, making the sum or difference undefined.


  
