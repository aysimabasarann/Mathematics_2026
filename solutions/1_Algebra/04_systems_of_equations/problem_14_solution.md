### Exercise 14. A Small Change in the Right-Hand Side

Compare the systems

$$
\begin{cases}
x+y=2, \\
2x-y=1, \\
3x=3
\end{cases}
$$

and

$$
\begin{cases}
x+y=2, \\
2x-y=1, \\
3x=3.1.
\end{cases}
$$

Check the consistency of each system and explain why a small change in one number can change the type of the system.

---

## Solution

### 1. Consistency Check for the First System

We write the augmented matrix for the first system:

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
2 & -1 & \mid & 1 \\
3 & 0 & \mid & 3 \\
\end{pmatrix}
$$

To eliminate the entries below the first pivot in column 1, apply the row operations $R_2 \leftarrow R_2 - 2R_1$ and $R_3 \leftarrow R_3 - 3R_1$:

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
0 & -3 & \mid & -3 \\
0 & -3 & \mid & -3 \\
\end{pmatrix}
$$

Eliminate the entry below the second pivot in column 2 by applying $R_3 \leftarrow R_3 - R_2$:

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
0 & -3 & \mid & -3 \\
0 & 0 & \mid & 0 \\
\end{pmatrix}
$$

The third row reduces to $0 = 0$, so there is no contradiction. From the second row, $-3y = -3 \implies y = 1$, and substituting into the first row gives $x + 1 = 2 \implies x = 1$. 

Therefore, the first system is **consistent** and has a **unique solution** $(x, y) = (1, 1)$.

### 2. Consistency Check for the Second System

We write the augmented matrix for the second system:

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
2 & -1 & \mid & 1 \\
3 & 0 & \mid & 3.1 \\
\end{pmatrix}
$$

Apply the exact same elimination steps $R_2 \leftarrow R_2 - 2R_1$ and $R_3 \leftarrow R_3 - 3R_1$:

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
0 & -3 & \mid & -3 \\
0 & -3 & \mid & -2.9 \\
\end{pmatrix}
$$

Eliminate the entry below the second pivot by applying $R_3 \leftarrow R_3 - R_2$:

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
0 & -3 & \mid & -3 \\
0 & 0 & \mid & 0.1 \\
\end{pmatrix}
$$

The third row corresponds to the equation $0x + 0y = 0.1 \implies 0 = 0.1$, which is a contradiction. 

Therefore, the second system is **inconsistent** and has **no solution**.

### 3. Why a Small Change Alters the System Type

In both systems, the first two equations ($x + y = 2$ and $2x - y = 1$) already uniquely determine a single intersection point in the plane, namely $(x, y) = (1, 1)$. Notice that adding the first two equations gives $(x + y) + (2x - y) = 2 + 1 \implies 3x = 3$.

- **In the first system:** The third equation $3x = 3$ is an exact linear combination of the first two equations. Geometrically, the third line passes directly through the existing intersection point $(1, 1)$ of the first two lines, keeping the overdetermined system consistent.
- **In the second system:** Changing $3$ to $3.1$ shifts the third line slightly to $x = \frac{3.1}{3} \approx 1.033$. Because an overdetermined system (3 equations in 2 unknowns) has zero degrees of freedom once two non-parallel lines intersect, even the smallest perturbation in the right-hand side moves the third line off the intersection point $(1, 1)$. With no single point lying on all three lines simultaneously, the system immediately changes from consistent to inconsistent.
