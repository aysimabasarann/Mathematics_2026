
### Exercise 3. Vector Normalization

Given the vector

$$
v=(3,4)
$$

**1. Finding the unit vector**

First, calculate the length of the vector.

$$
\begin{aligned}
\|v\| &= \sqrt{3^2+4^2} \\
&= \sqrt{9+16} \\
&= \sqrt{25} \\
&= 5
\end{aligned}
$$

A unit vector with the same direction and orientation is obtained by dividing the original vector by its length.

$$
\begin{aligned}
e &= \frac{v}{\|v\|} \\
&= \frac{(3,4)}{5} \\
&= \left(\frac{3}{5},\frac{4}{5}\right)
\end{aligned}
$$

**2. Verification of the unit vector**

The length of a unit vector must be equal to 1.

$$
\begin{aligned}
\|e\| &= \sqrt{\left(\frac{3}{5}\right)^2+\left(\frac{4}{5}\right)^2} \\
&= \sqrt{\frac{9}{25}+\frac{16}{25}} \\
&= \sqrt{\frac{25}{25}} \\
&= 1
\end{aligned}
$$

Therefore, $e$ is a unit vector.

**3. Reconstructing the original vector**

Using the relation $v=\|v\|e$:

$$
\begin{aligned}
v &= 5\left(\frac{3}{5},\frac{4}{5}\right) \\
&= (3,4)
\end{aligned}
$$

The original vector is reconstructed correctly.

**4. Geometric interpretation**

Normalization changes the length of a nonzero vector to 1 while preserving its direction and orientation. The original vector and the unit vector point in the same direction, but they have different lengths.

