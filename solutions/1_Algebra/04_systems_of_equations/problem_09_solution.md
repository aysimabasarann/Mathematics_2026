### Exercise 9. A System from a Sum Condition

Find numbers $x,y$ satisfying

$$x+y=10,\qquad 2x+5y=32.$$

Solve the system and explain geometrically why the solution is unique.

---

## Solution

### 1. Solving the System

We write the given conditions as a system of linear equations:

$$\begin{cases} x + y = 10, \\ 2x + 5y = 32. \end{cases}$$

Form the corresponding augmented matrix:

$$\begin{pmatrix} 1 & 1 & \mid & 10 \\ 2 & 5 & \mid & 32 \\ \end{pmatrix}$$

To eliminate the entry below the pivot in the first column, apply the row operation $R_2 \leftarrow R_2 - 2R_1$:

$$\begin{pmatrix} 1 & 1 & \mid & 10 \\ 0 & 3 & \mid & 12 \\ \end{pmatrix}$$

Divide the second row by $3$ ($R_2 \leftarrow \frac{1}{3}R_2$) to obtain a leading $1$:

$$\begin{pmatrix} 1 & 1 & \mid & 10 \\ 0 & 1 & \mid & 4 \\ \end{pmatrix}$$

From the second row, we read directly:

$$y = 4$$

Substitute $y = 4$ back into the first equation $x + y = 10$:

$$x + 4 = 10 \implies x = 6$$

Thus, the numbers satisfying both conditions are $x = 6$ and $y = 4$.

### 2. Geometric Explanation of Uniqueness

Each linear equation in two variables represents a straight line in the Cartesian plane $\mathbb{R}^2$. Rewriting both equations in slope-intercept form ($y = mx + c$) reveals their slopes:

- **First equation ($x + y = 10$):**

$$y = -x + 10 \quad (\text{slope } m_1 = -1)$$

- **Second equation ($2x + 5y = 32$):**

$$y = -\frac{2}{5}x + \frac{32}{5} \quad (\text{slope } m_2 = -\frac{2}{5})$$

Because the two lines have different slopes ($m_1 = -1 \neq -\frac{2}{5} = m_2$), they are neither parallel nor coincident. In Euclidean plane geometry, two non-parallel lines must intersect at **exactly one point**. The coordinates of this unique intersection point are $(6, 4)$, which corresponds to the unique algebraic solution of the system.
