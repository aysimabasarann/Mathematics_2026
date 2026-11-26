### Exercise 12. Intersection Line of Two Planes

#### Question
Find a parametric equation of the line that is the intersection of

$$
x+y+z=3,\qquad x-y+z=1.
$$

Find its direction vector in two ways: from the system of equations and from the cross product of the normal vectors. Compare the results.

#### Solution
Given planes are

$$
\Pi_1: x + y + z = 3, \qquad \Pi_2: x - y + z = 1.
$$

**1. Parametric Equation via the System of Equations**
Adding the two plane equations eliminates $y$:

$$
\begin{aligned}
(x + y + z) + (x - y + z) &= 3 + 1 \\
2x + 2z &= 4 \\
x + z &= 2 \implies x = 2 - z
\end{aligned}
$$

Substituting $x = 2 - z$ into the first equation $\Pi_1$:

$$
\begin{aligned}
(2 - z) + y + z &= 3 \\
2 + y &= 3 \\
y &= 1
\end{aligned}
$$

Letting $z = t$ (where $t \in \mathbb{R}$), the coordinates are expressed as

$$
\begin{cases}
x = 2 - t, \\
y = 1, \\
z = t.
\end{cases}
$$

Thus, the parametric equation of the intersection line is

$$
(x, y, z) = (2, 1, 0) + t(-1, 0, 1), \qquad t \in \mathbb{R},
$$

yielding a direction vector $v_1 = (-1, 0, 1)$.

**2. Finding the Direction Vector via Cross Product of Normals**
The normal vectors of the planes are

$$
n_1 = (1, 1, 1), \qquad n_2 = (1, -1, 1).
$$

The intersection line lies in both planes, meaning its direction vector $v_2$ must be perpendicular to both $n_1$ and $n_2$. We find $v_2$ using their cross product:

$$
\begin{aligned}
v_2 &= n_1 \times n_2 \\
    &= ((1)(1) - (1)(-1),\; (1)(1) - (1)(1),\; (1)(-1) - (1)(1)) \\
    &= (1 + 1,\; 1 - 1,\; -1 - 1) \\
    &= (2, 0, -2)
\end{aligned}
$$

**3. Comparison of Results**
The direction vector from the system is $v_1 = (-1, 0, 1)$, while the cross product yields $v_2 = (2, 0, -2)$. Comparing the two vectors shows that

$$
v_2 = -2 v_1.
$$

Since $v_2$ is a nonzero scalar multiple of $v_1$, both direction vectors define the exact same line of direction in space. The algebraic approach and the cross product of normal vectors are fully equivalent.
