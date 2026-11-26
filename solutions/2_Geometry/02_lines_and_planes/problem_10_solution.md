### Exercise 10. Projection of a Point onto a Plane

#### Question
Find the orthogonal projection of $P=(2,1,3)$ onto the plane $x+y+z=3$, and then find the reflection of $P$ across this plane. Check that the midpoint of the segment joining the point and its reflection lies on the plane.

#### Solution
Given point and plane are

$$
P = (2, 1, 3), \qquad \Pi: x + y + z = 3.
$$

**1. Orthogonal Projection $Q$ onto the Plane**
A normal vector to the plane $\Pi$ is $n = (1, 1, 1)$. The line passing through $P = (2, 1, 3)$ in the direction of $n$ has parametric equation

$$
\begin{cases}
x = 2 + t, \\
y = 1 + t, \\
z = 3 + t.
\end{cases}
$$

The orthogonal projection $Q$ is the intersection of this normal line with the plane $\Pi$. Substituting the parametric coordinates into $x + y + z = 3$:

$$
\begin{aligned}
(2 + t) + (1 + t) + (3 + t) &= 3 \\
6 + 3t &= 3 \\
3t &= -3 \\
t &= -1
\end{aligned}
$$

Substituting $t = -1$ into the line equation gives the projection $Q$:

$$
\begin{aligned}
Q &= (2 + (-1),\; 1 + (-1),\; 3 + (-1)) \\
  &= (1, 0, 2)
\end{aligned}
$$

**2. Reflection $P'$ Across the Plane**
Since $Q$ is the midpoint between $P$ and its reflection $P'$, we have $\overrightarrow{QP'} = -\overrightarrow{QP} = \overrightarrow{PQ}$, or equivalently $P' = 2Q - P$:

$$
\begin{aligned}
P' &= 2(1, 0, 2) - (2, 1, 3) \\
   &= (2, 0, 4) - (2, 1, 3) \\
   &= (0, -1, 1)
\end{aligned}
$$

**3. Verification via the Midpoint**
Computing the midpoint $M$ of the segment joining $P = (2, 1, 3)$ and $P' = (0, -1, 1)$:

$$
\begin{aligned}
M &= \left(\frac{2 + 0}{2},\; \frac{1 + (-1)}{2},\; \frac{3 + 1}{2}\right) \\
  &= \left(\frac{2}{2},\; \frac{0}{2},\; \frac{4}{2}\right) \\
  &= (1, 0, 2)
\end{aligned}
$$

Note that $M = Q$. Substituting $M = (1, 0, 2)$ into the plane equation $x + y + z = 3$:

$$
1 + 0 + 2 = 3
$$

The midpoint lies directly on the plane $\Pi$, confirming both the projection and the reflection.
