### Exercise 13. Closest Point on a Plane

#### Question
Find the point on the plane $x+2y+2z=4$ closest to $P=(3,0,0)$. Give the distance and check that the segment joining the two points is perpendicular to the plane.

#### Solution
Given point and plane are

$$
P = (3, 0, 0), \qquad \Pi: x + 2y + 2z = 4.
$$

**1. Closest Point $Q$ on the Plane**
A normal vector to the plane $\Pi$ is $n = (1, 2, 2)$. The line passing through $P = (3, 0, 0)$ in the direction of $n$ has parametric equations

$$
\begin{cases}
x = 3 + t, \\
y = 2t, \\
z = 2t.
\end{cases}
$$

The closest point $Q$ on $\Pi$ is the intersection of this perpendicular line with the plane. Substituting into $x + 2y + 2z = 4$:

$$
\begin{aligned}
(3 + t) + 2(2t) + 2(2t) &= 4 \\
3 + t + 4t + 4t &= 4 \\
3 + 9t &= 4 \\
9t &= 1 \\
t &= \frac{1}{9}
\end{aligned}
$$

Substituting $t = \frac{1}{9}$ back into the parametric equations gives $Q$:

$$
\begin{aligned}
Q &= \left(3 + \frac{1}{9},\; 2\left(\frac{1}{9}\right),\; 2\left(\frac{1}{9}\right)\right) \\
  &= \left(\frac{28}{9},\; \frac{2}{9},\; \frac{2}{9}\right)
\end{aligned}
$$

**2. Distance from $P$ to the Plane**
The displacement vector from $P$ to $Q$ is

$$
\begin{aligned}
\overrightarrow{PQ} &= Q - P \\
                    &= \left(\frac{28}{9} - 3,\; \frac{2}{9} - 0,\; \frac{2}{9} - 0\right) \\
                    &= \left(\frac{1}{9},\; \frac{2}{9},\; \frac{2}{9}\right)
\end{aligned}
$$

Computing the distance $d = \|\overrightarrow{PQ}\|$:

$$
\begin{aligned}
d &= \sqrt{\left(\frac{1}{9}\right)^2 + \left(\frac{2}{9}\right)^2 + \left(\frac{2}{9}\right)^2} \\
  &= \sqrt{\frac{1}{81} + \frac{4}{81} + \frac{4}{81}} \\
  &= \sqrt{\frac{9}{81}} \\
  &= \frac{3}{9} \\
  &= \frac{1}{3}
\end{aligned}
$$

**3. Verification of Perpendicularity**
Notice that the vector connecting $P$ and $Q$ is

$$
\overrightarrow{PQ} = \left(\frac{1}{9}, \frac{2}{9}, \frac{2}{9}\right) = \frac{1}{9}(1, 2, 2) = \frac{1}{9}n.
$$

Because $\overrightarrow{PQ}$ is a nonzero scalar multiple of the plane's normal vector $n = (1, 2, 2)$, the segment $PQ$ is verified to be perpendicular to the plane $\Pi$.
