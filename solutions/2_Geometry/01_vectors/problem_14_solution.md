### Exercise 14. Closest Point on a Line

#### Question
Given a point $P=(4,1)$ and a line through the origin with direction $v=(1,2)$. Using projection, find the closest point on the line, the distance from $P$ to the line, and verify that the appropriate vector is perpendicular to the direction of the line.

#### Solution
Given point is $P = (4, 1)$ and the line through the origin $O = (0, 0)$ has direction vector $v = (1, 2)$.

**1. Closest Point on the Line**
Let $u = \overrightarrow{OP} = (4, 1)$. The closest point $Q$ on the line corresponds to the orthogonal projection of $u$ onto $v$:

$$
\overrightarrow{OQ} = \mathrm{proj}_v\,u = \frac{u \cdot v}{v \cdot v} v
$$

Computing the dot products:

$$
\begin{aligned}
u \cdot v &= (4)(1) + (1)(2) \\
          &= 4 + 2 \\
          &= 6
\end{aligned}
$$

$$
\begin{aligned}
v \cdot v &= (1)(1) + (2)(2) \\
          &= 1 + 4 \\
          &= 5
\end{aligned}
$$

Substituting into the projection formula:

$$
\begin{aligned}
\overrightarrow{OQ} &= \frac{6}{5}(1, 2) \\
                    &= \left(\frac{6}{5}, \frac{12}{5}\right)
\end{aligned}
$$

Thus, the closest point on the line is

$$
Q = \left(\frac{6}{5}, \frac{12}{5}\right).
$$

**2. Distance from $P$ to the Line**
The shortest distance is the length of the perpendicular residual vector $r = \overrightarrow{QP} = P - Q$:

$$
\begin{aligned}
r &= (4, 1) - \left(\frac{6}{5}, \frac{12}{5}\right) \\
  &= \left(4 - \frac{6}{5},\; 1 - \frac{12}{5}\right) \\
  &= \left(\frac{14}{5}, -\frac{7}{5}\right)
\end{aligned}
$$

Computing the length of $r$:

$$
\begin{aligned}
d &= \|r\| \\
  &= \sqrt{\left(\frac{14}{5}\right)^2 + \left(-\frac{7}{5}\right)^2} \\
  &= \sqrt{\frac{196}{25} + \frac{49}{25}} \\
  &= \sqrt{\frac{245}{25}} \\
  &= \frac{7\sqrt{5}}{5}
\end{aligned}
$$

**3. Verification of Perpendicularity**
Checking that the connecting vector $r$ is perpendicular to the direction vector $v$:

$$
\begin{aligned}
r \cdot v &= \left(\frac{14}{5}\right)(1) + \left(-\frac{7}{5}\right)(2) \\
          &= \frac{14}{5} - \frac{14}{5} \\
          &= 0
\end{aligned}
$$

Since $r \cdot v = 0$, the vector $\overrightarrow{QP}$ is verified to be perpendicular to the direction of the line.


