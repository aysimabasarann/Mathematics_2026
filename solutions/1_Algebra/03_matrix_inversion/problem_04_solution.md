### Exercise 4. Gauss–Jordan

Find $A^{-1}$ using the Gauss–Jordan method for

$$
A=
\begin{pmatrix}
1 & 2 \\
3 & 5 \\
\end{pmatrix}
$$

Show the augmented matrix $[A\mid I]$ after successive operations and explain why obtaining $I$ on the left gives the inverse on the right.

---

## Solution

### 1. Applying Gauss–Jordan Elimination

We set up the augmented matrix $[A \mid I]$ by placing the identity matrix of the same size next to $A$:

$$
\begin{pmatrix}
1 & 2 & \mid & 1 & 0 \\
3 & 5 & \mid & 0 & 1 \\
\end{pmatrix}
$$

Next, we apply elementary row operations to transform the left side into the identity matrix $I$.

**Step 1:** Eliminate the entry below the pivot in the first column by applying $R_2 \leftarrow R_2 - 3R_1$:

$$
\begin{pmatrix}
1 & 2 & \mid & 1 & 0 \\
0 & -1 & \mid & -3 & 1 \\
\end{pmatrix}
$$

**Step 2:** Scale the second row to make the pivot equal to $1$ by applying $R_2 \leftarrow -R_2$:

$$
\begin{pmatrix}
1 & 2 & \mid & 1 & 0 \\
0 & 1 & \mid & 3 & -1 \\
\end{pmatrix}
$$

**Step 3:** Eliminate the entry above the pivot in the second column by applying $R_1 \leftarrow R_1 - 2R_2$:

$$
\begin{pmatrix}
1 & 0 & \mid & -5 & 2 \\
0 & 1 & \mid & 3 & -1 \\
\end{pmatrix}
$$

Since the left side has been successfully transformed into the identity matrix $I$, the right side now contains the inverse matrix $A^{-1}$:

$$
A^{-1} =
\begin{pmatrix}
-5 & 2 \\
3 & -1 \\
\end{pmatrix}
$$

### 2. Meaning of the Method

Each elementary row operation corresponds to left-multiplication by an elementary matrix. Transforming the augmented matrix $[A \mid I]$ into $[I \mid A^{-1}]$ means that a sequence of elementary matrices $E_k \cdots E_2 E_1$ has been applied such that:

$$
(E_k \cdots E_2 E_1) A = I
$$

By definition of the inverse matrix, the product of these elementary matrices must equal $A^{-1}$. When the exact same sequence of operations is simultaneously applied to the identity matrix on the right, we obtain:

$$
(E_k \cdots E_2 E_1) I = A^{-1}
$$

Thus, reducing the left side to $I$ automatically accumulates the inverse matrix on the right side.

 

 
