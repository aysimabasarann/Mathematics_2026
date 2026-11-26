### Exercise 3. Plane Through a Point with a Given Normal Vector

#### Question
Find the equation of the plane through $P=(1,-2,3)$ and perpendicular to $n=(2,1,-1)$. Check the result by substituting the point $P$ and explain the role of the normal vector.

#### Solution
Given point and normal vector are

$$
P = (1, -2, 3), \qquad n = (2, 1, -1).
$$

**1. Equation of the Plane**
A point $X = (x, y, z)$ lies on the plane if and only if the displacement vector $\overrightarrow{PX} = X - P$ is perpendicular to the normal vector $n$:

$$
n \cdot (X - P) = 0
$$

Substituting the coordinates of $P$ and $n$:

$$
\begin{aligned}
2(x - 1) + 1(y - (-2)) - 1(z - 3) &= 0 \\
2(x - 1) + (y + 2) - (z - 3) &= 0 \\
2x - 2 + y + 2 - z + 3 &= 0 \\
2x + y - z + 3 &= 0
\end{aligned}
$$

Equivalently, the equation of the plane is

$$
2x + y - z = -3.
$$

**2. Verification by Substituting $P$**
Substituting $P = (1, -2, 3)$ into the left-hand side of $2x + y - z + 3 = 0$:

$$
\begin{aligned}
2(1) + (-2) - (3) + 3 &= 2 - 2 - 3 + 3 \\
                      &= 0
\end{aligned}
$$

Since the equation holds, point $P$ lies on the plane.

**3. Role of the Normal Vector**
The normal vector $n = (2, 1, -1)$ fixes the spatial orientation (tilt) of the plane by defining the unique direction perpendicular to every vector lying inside the plane. Its components $(2, 1, -1)$ appear directly as the coefficients of $x$, $y$, and $z$ in the general linear equation of the plane, while the point $P$ determines the specific shift (constant term) that places the plane in space.
