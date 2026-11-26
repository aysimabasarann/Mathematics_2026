
### Exercise 14. Closest Point on a Line

Given the point and the direction vector

$$
P=(4,1),\qquad v=(1,2)
$$

The line passes through the origin and has direction vector $v$.

**1. Finding the closest point on the line**

The closest point on the line is the projection of $P$ onto the direction vector $v$.

The projection formula is

$$
Q=\mathrm{proj}_v\,P=\frac{P\cdot v}{v\cdot v}v
$$

First, calculate the dot product.

$$
\begin{aligned}
P\cdot v &= 4\cdot 1+1\cdot 2 \\
&= 4+2 \\
&= 6
\end{aligned}
$$

Calculate the squared length of $v$.

$$
\begin{aligned}
v\cdot v &= 1^2+2^2 \\
&= 1+4 \\
&= 5
\end{aligned}
$$

Substitute these values into the projection formula.

$$
\begin{aligned}
Q &= \frac{6}{5}(1,2) \\
&= \left(\frac{6}{5},\frac{12}{5}\right)
\end{aligned}
$$

Therefore, the closest point on the line is

$$
Q=\left(\frac{6}{5},\frac{12}{5}\right)
$$

**2. Computing the distance from the point to the line**

The distance is the length of the perpendicular vector from $P$ to $Q$.

$$
\begin{aligned}
r &= P-Q \\
&= (4,1)-\left(\frac{6}{5},\frac{12}{5}\right) \\
&= \left(\frac{20}{5}-\frac{6}{5},\frac{5}{5}-\frac{12}{5}\right) \\
&= \left(\frac{14}{5},-\frac{7}{5}\right)
\end{aligned}
$$

Calculate its length.

$$
\begin{aligned}
d(P,Q) &= \|r\| \\
&= \sqrt{\left(\frac{14}{5}\right)^2+\left(-\frac{7}{5}\right)^2} \\
&= \sqrt{\frac{196}{25}+\frac{49}{25}} \\
&= \sqrt{\frac{245}{25}} \\
&= \frac{7\sqrt{5}}{5}
\end{aligned}
$$

Therefore, the distance from $P$ to the line is

$$
d=\frac{7\sqrt{5}}{5}
$$

**3. Verification of perpendicularity**

The shortest distance from a point to a line is perpendicular to the direction vector of the line.

This can be verified by calculating the dot product of $r$ and $v$.

$$
\begin{aligned}
r\cdot v &= \left(\frac{14}{5},-\frac{7}{5}\right)\cdot(1,2) \\
&= \frac{14}{5}-\frac{14}{5} \\
&= 0
\end{aligned}
$$

Since the dot product is zero, the vector $r$ is perpendicular to the direction vector $v$.

Therefore, $Q$ is the closest point on the line to $P$, and the calculated distance is the shortest possible distance.

