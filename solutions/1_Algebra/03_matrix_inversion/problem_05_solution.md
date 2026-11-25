### Exercise 5. A 3×3 Matrix

Use Gauss–Jordan elimination to find the inverse of

$$
A=
\begin{pmatrix}
1 & 1 & 0 \\
0 & 1 & 1 \\
1 & 0 & 1 \\
\end{pmatrix}
$$

Check the result by multiplication.

---

## Solution

### 1. Applying Gauss–Jordan Elimination

We set up the augmented matrix $[A \mid I]$:

$$
\begin{pmatrix}
1 & 1 & 0 & \mid & 1 & 0 & 0 \\
0 & 1 & 1 & \mid & 0 & 1 & 0 \\
1 & 0 & 1 & \mid & 0 & 0 & 1 \\
\end{pmatrix}
$$

We apply elementary row operations to reduce the left side to the identity matrix $I$.

**Step 1:** Eliminate the entry below the pivot in the first column by applying $R_3 \leftarrow R_3 - R_1$:

$$
\begin{pmatrix}
1 & 1 & 0 & \mid & 1 & 0 & 0 \\
0 & 1 & 1 & \mid & 0 & 1 & 0 \\
0 & -1 & 1 & \mid & -1 & 0 & 1 \\
\end{pmatrix}
$$

**Step 2:** Eliminate the entry below the pivot in the second column by applying $R_3 \leftarrow R_3 + R_2$:

$$
\begin{pmatrix}
1 & 1 & 0 & \mid & 1 & 0 & 0 \\
0 & 1 & 1 & \mid & 0 & 1 & 0 \\
0 & 0 & 2 & \mid & -1 & 1 & 1 \\
\end{pmatrix}
$$

**Step 3:** Scale the third row to obtain a leading $1$ by applying $R_3 \leftarrow \frac{1}{2}R_3$:

$$
\begin{pmatrix}
1 & 1 & 0 & \mid & 1 & 0 & 0 \\
0 & 1 & 1 & \mid & 0 & 1 & 0 \\
0 & 0 & 1 & \mid & -\frac{1}{2} & \frac{1}{2} & \frac{1}{2} \\
\end{pmatrix}
$$

**Step 4:** Eliminate entries above the pivot in the third column using $R_2 \leftarrow R_2 - R_3$:

$$
\begin{pmatrix}
1 & 1 & 0 & \mid & 1 & 0 & 0 \\
0 & 1 & 0 & \mid & \frac{1}{2} & \frac{1}{2} & -\frac{1}{2} \\
0 & 0 & 1 & \mid & -\frac{1}{2} & \frac{1}{2} & \frac{1}{2} \\
\end{pmatrix}
$$

**Step 5:** Eliminate the entry above the pivot in the second column using $R_1 \leftarrow R_1 - R_2$:

$$
\begin{pmatrix}
1 & 0 & 0 & \mid & \frac{1}{2} & -\frac{1}{2} & \frac{1}{2} \\
0 & 1 & 0 & \mid & \frac{1}{2} & \frac{1}{2} & -\frac{1}{2} \\
0 & 0 & 1 & \mid & -\frac{1}{2} & \frac{1}{2} & \frac{1}{2} \\
\end{pmatrix}
$$

Thus, the inverse matrix is:

$$
A^{-1} =
\begin{pmatrix}
\frac{1}{2} & -\frac{1}{2} & \frac{1}{2} \\
\frac{1}{2} & \frac{1}{2} & -\frac{1}{2} \\
-\frac{1}{2} & \frac{1}{2} & \frac{1}{2} \\
\end{pmatrix}
$$

### 2. Verification by Multiplication

We check the result by computing the product $AA^{-1}$:

$$
\begin{aligned}
AA^{-1} &=
\begin{pmatrix}
1 & 1 & 0 \\
0 & 1 & 1 \\
1 & 0 & 1 \\
\end{pmatrix}
\begin{pmatrix}
\frac{1}{2} & -\frac{1}{2} & \frac{1}{2} \\
\frac{1}{2} & \frac{1}{2} & -\frac{1}{2} \\
-\frac{1}{2} & \frac{1}{2} & \frac{1}{2} \\
\end{pmatrix} \\
&=
\begin{pmatrix}
\frac{1}{2} + \frac{1}{2} + 0 & -\frac{1}{2} + \frac{1}{2} + 0 & \frac{1}{2} - \frac{1}{2} + 0 \\
0 + \frac{1}{2} - \frac{1}{2} & 0 + \frac{1}{2} + \frac{1}{2} & 0 - \frac{1}{2} + \frac{1}{2} \\
\frac{1}{2} + 0 - \frac{1}{2} & -\frac{1}{2} + 0 + \frac{1}{2} & \frac{1}{2} + 0 + \frac{1}{2} \\
\end{pmatrix} \\
&=
\begin{pmatrix}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1 \\
\end{pmatrix}
= I
\end{aligned}
$$

Since $AA^{-1} = I$, the computed inverse is correct.





