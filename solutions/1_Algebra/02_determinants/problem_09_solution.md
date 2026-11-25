### Exercise 9. Area and the Determinant

The vectors

$$
u=
\begin{pmatrix}
3 \\
1 \\
\end{pmatrix},\qquad v=
\begin{pmatrix}
1 \\
4 \\
\end{pmatrix}
$$

span a parallelogram. Compute its area using a determinant. Then reverse the order of the vectors and explain what changes in the determinant and what does not change in the area.

---

## Solution

### 1. Computing the Area Using a Determinant

In $\mathbb{R}^2$, the area of the parallelogram spanned by two vectors $u$ and $v$ is equal to the absolute value of the determinant of the $2 \times 2$ matrix formed by placing these vectors as columns (or rows):

$$
A =
\begin{pmatrix}
3 & 1 \\
1 & 4 \\
\end{pmatrix}
$$

Computing the determinant of $A$:

$$
\det A = (3)(4) - (1)(1) = 12 - 1 = 11
$$

Taking the absolute value gives the area of the parallelogram:

$$
\mathrm{Area} = |\det A| = |11| = 11
$$

### 2. Reversing the Order of the Vectors

If we reverse the order of the vectors so that $v$ is placed first and $u$ second, we form a new matrix $B$:

$$
B =
\begin{pmatrix}
1 & 3 \\
4 & 1 \\
\end{pmatrix}
$$

Computing the determinant of $B$:

$$
\det B = (1)(1) - (3)(4) = 1 - 12 = -11
$$

### 3. Explanation of What Changes and What Remains Unchanged

* **What changes (the sign of the determinant):** Reversing the order of the vectors swaps the two columns of the matrix. Swapping two columns (or two rows) multiplies the determinant by $-1$, changing its value from $+11$ to $-11$. Geometrically, this reflects a reversal of orientation from counterclockwise to clockwise.
* **What does not change (the area):** Area is a non-negative geometric measure defined as the absolute value of the determinant. Since $|-11| = |11| = 11$, the area of the parallelogram remains completely unchanged.

 
