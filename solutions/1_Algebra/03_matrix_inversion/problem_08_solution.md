### Exercise 8. Inverse of a Transformation

The matrix

$$
S=
\begin{pmatrix}
2 & 0 \\
0 & \frac{1}{2} \\
\end{pmatrix}
$$

describes a scaling of the plane. Find $S^{-1}$ and explain geometrically what the inverse transformation does. Check the action of the pair $S, S^{-1}$ on one simple vector.

---

## Solution

### 1. Finding $S^{-1}$

To find the inverse of the diagonal matrix $S$, we apply the $2 \times 2$ inverse formula. First, we compute the determinant of $S$:

$$
\det S = (2)\left(\frac{1}{2}\right) - (0)(0) = 1 - 0 = 1
$$

Since $\det S = 1 \neq 0$, the inverse exists. Applying the formula:

$$
S^{-1} = \frac{1}{1}
\begin{pmatrix}
\frac{1}{2} & 0 \\
0 & 2 \\
\end{pmatrix}
$$

Simplifying the scalar multiplication:

$$
S^{-1} =
\begin{pmatrix}
\frac{1}{2} & 0 \\
0 & 2 \\
\end{pmatrix}
$$

### 2. Geometric Interpretation of the Inverse Transformation

The original matrix $S$ stretches the plane horizontally by a factor of $2$ and compresses it vertically by a factor of $\frac{1}{2}$. 

The inverse transformation $S^{-1}$ does the exact opposite ("undoes" the scaling): it compresses the plane horizontally by a factor of $\frac{1}{2}$ and stretches it vertically by a factor of $2$.

### 3. Checking the Action on a Simple Vector

Let us test the pair $S$ and $S^{-1}$ on a simple vector $v = \begin{pmatrix} 4 \\ 3 \end{pmatrix}$.

First, apply $S$ to $v$:

$$
Sv =
\begin{pmatrix}
2 & 0 \\
0 & \frac{1}{2} \\
\end{pmatrix}
\begin{pmatrix}
4 \\
3 \\
\end{pmatrix}
$$

Writing out the multiplication:

$$
Sv =
\begin{pmatrix}
(2)(4) \\
\left(\frac{1}{2}\right)(3) \\
\end{pmatrix}
$$

Evaluating the entries:

$$
Sv =
\begin{pmatrix}
8 \\
\frac{3}{2} \\
\end{pmatrix}
$$

Next, apply $S^{-1}$ to the resulting vector:

$$
S^{-1}(Sv) =
\begin{pmatrix}
\frac{1}{2} & 0 \\
0 & 2 \\
\end{pmatrix}
\begin{pmatrix}
8 \\
\frac{3}{2} \\
\end{pmatrix}
$$

Writing out the multiplication:

$$
S^{-1}(Sv) =
\begin{pmatrix}
\left(\frac{1}{2}\right)(8) \\
(2)\left(\frac{3}{2}\right) \\
\end{pmatrix}
$$

Evaluating the entries:

$$
S^{-1}(Sv) =
\begin{pmatrix}
4 \\
3 \\
\end{pmatrix}
= v
$$

Applying $S$ followed by $S^{-1}$ successfully restores the original vector $v$.

