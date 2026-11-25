### Exercise 13. Undoing a Composite Transformation

The matrices

$$
S=
\begin{pmatrix}
2 & 0 \\
0 & 1 \\
\end{pmatrix},\qquad H=
\begin{pmatrix}
1 & 1 \\
0 & 1 \\
\end{pmatrix}
$$

describe nonuniform scaling and shear. For $T=HS$, find $T^{-1}$ in two ways:

1. first compute $T$, then its inverse,
2. use $(HS)^{-1}=S^{-1}H^{-1}$.

Compare the results. Additionally compute $H^{-1}S^{-1}$ and verify that the incorrect order gives a different matrix. Explain the rule: “when undoing a composition of operations, we undo them from the end.”

---

## Solution

### 1. Finding $T^{-1}$ by First Computing $T$

First, we compute the composite transformation matrix $T = HS$:

$$
T =
\begin{pmatrix}
1 & 1 \\
0 & 1 \\
\end{pmatrix}
\begin{pmatrix}
2 & 0 \\
0 & 1 \\
\end{pmatrix}
$$

Writing out the multiplication of entries in separate display blocks:

$$
T =
\begin{pmatrix}
(1)(2) + (1)(0) & (1)(0) + (1)(1) \\
(0)(2) + (1)(0) & (0)(0) + (1)(1) \\
\end{pmatrix}
$$

Simplifying the entries:

$$
T =
\begin{pmatrix}
2 + 0 & 0 + 1 \\
0 + 0 & 0 + 1 \\
\end{pmatrix}
$$

Evaluating the sums:

$$
T =
\begin{pmatrix}
2 & 1 \\
0 & 1 \\
\end{pmatrix}
$$

Next, we find the inverse of $T$ using the $2 \times 2$ inverse formula. The determinant is:

$$
\det T = (2)(1) - (1)(0) = 2
$$

Applying the inverse formula:

$$
T^{-1} = \frac{1}{2}
\begin{pmatrix}
1 & -1 \\
0 & 2 \\
\end{pmatrix}
$$

Distributing the scalar $\frac{1}{2}$:

$$
T^{-1} =
\begin{pmatrix}
\frac{1}{2} & -\frac{1}{2} \\
0 & 1 \\
\end{pmatrix}
$$

### 2. Finding $T^{-1}$ Using $(HS)^{-1} = S^{-1}H^{-1}$

First, we find the individual inverses $S^{-1}$ and $H^{-1}$:

For matrix $S$, since it is diagonal, we invert its diagonal entries:

$$
S^{-1} =
\begin{pmatrix}
\frac{1}{2} & 0 \\
0 & 1 \\
\end{pmatrix}
$$

For matrix $H$, using the $2 \times 2$ inverse formula (determinant $\det H = (1)(1) - (1)(0) = 1$):

$$
H^{-1} =
\begin{pmatrix}
1 & -1 \\
0 & 1 \\
\end{pmatrix}
$$

Now, we compute the product $S^{-1}H^{-1}$:

$$
S^{-1}H^{-1} =
\begin{pmatrix}
\frac{1}{2} & 0 \\
0 & 1 \\
\end{pmatrix}
\begin{pmatrix}
1 & -1 \\
0 & 1 \\
\end{pmatrix}
$$

Writing out the matrix multiplication:

$$
S^{-1}H^{-1} =
\begin{pmatrix}
\left(\frac{1}{2}\right)(1) + (0)(0) & \left(\frac{1}{2}\right)(-1) + (0)(1) \\
(0)(1) + (1)(0) & (0)(-1) + (1)(1) \\
\end{pmatrix}
$$

Simplifying the entries:

$$
S^{-1}H^{-1} =
\begin{pmatrix}
\frac{1}{2} + 0 & -\frac{1}{2} + 0 \\
0 + 0 & 0 + 1 \\
\end{pmatrix}
$$

Evaluating the sums:

$$
S^{-1}H^{-1} =
\begin{pmatrix}
\frac{1}{2} & -\frac{1}{2} \\
0 & 1 \\
\end{pmatrix}
$$

Both methods yield the exact same result: $T^{-1} = \begin{pmatrix} \frac{1}{2} & -\frac{1}{2} \\ 0 & 1 \end{pmatrix}$.

### 3. Computing $H^{-1}S^{-1}$ (Incorrect Order)

To verify what happens in the wrong order, we compute $H^{-1}S^{-1}$:

$$
H^{-1}S^{-1} =
\begin{pmatrix}
1 & -1 \\
0 & 1 \\
\end{pmatrix}
\begin{pmatrix}
\frac{1}{2} & 0 \\
0 & 1 \\
\end{pmatrix}
$$

Writing out the multiplication:

$$
H^{-1}S^{-1} =
\begin{pmatrix}
(1)\left(\frac{1}{2}\right) + (-1)(0) & (1)(0) + (-1)(1) \\
(0)\left(\frac{1}{2}\right) + (1)(0) & (0)(0) + (1)(1) \\
\end{pmatrix}
$$

Simplifying the entries:

$$
H^{-1}S^{-1} =
\begin{pmatrix}
\frac{1}{2} + 0 & 0 - 1 \\
0 + 0 & 0 + 1 \\
\end{pmatrix}
$$

Evaluating the sums:

$$
H^{-1}S^{-1} =
\begin{pmatrix}
\frac{1}{2} & -1 \\
0 & 1 \\
\end{pmatrix}
$$

Comparing this with $T^{-1}$, we see that $H^{-1}S^{-1} \neq S^{-1}H^{-1}$. The incorrect order gives a completely different matrix.

### 4. Explanation of the Rule

**Rule explanation:** Matrix multiplication represents the sequential application of linear transformations. When we apply transformation $S$ first and then transformation $H$, the combined operation is written from right to left as $T = HS$. To undo this composite operation, we must reverse the steps in the exact opposite order: we must first undo the last applied operation ($H$, via $H^{-1}$), and then undo the first applied operation ($S$, via $S^{-1}$). Hence, the inverse of a product is always given by $(HS)^{-1} = S^{-1}H^{-1}$.






 
 

 




