### Exercise 6. Angle Between Planes

#### Question
Given

$$
\Pi_1:x+y+z=1,\qquad \Pi_2:x-y=2.
$$

First use the normal vectors to decide whether the planes are parallel. If not, compute the angle between them and explain why the normal vectors alone are enough for this calculation.

#### Solution
The given planes are

$$
\Pi_1: x + y + z = 1, \qquad \Pi_2: x - y = 2.
$$

**1. Normal Vectors and Parallelism Check**
Reading the coefficients of $x$, $y$, and $z$ directly gives the normal vectors of the planes:

$$
n_1 = (1, 1, 1), \qquad n_2 = (1, -1, 0).
$$

Two planes are parallel if and only if their normal vectors are scalar multiples of each other. Since there is no scalar $k$ such that $(1, 1, 1) = k(1, -1, 0)$ (for example, the third component of $n_2$ is $0$ while that of $n_1$ is $1$), the normal vectors are not collinear. Thus, the planes $\Pi_1$ and $\Pi_2$ are **not parallel** (they intersect along a line).

**2. Angle Between the Planes**
The acute angle $\theta \in [0^\circ, 90^\circ]$ between two planes equals the acute angle between their normal vectors:

$$
\cos\theta = \frac{|n_1 \cdot n_2|}{\|n_1\|\,\|n_2\|}
$$

Computing the dot product and lengths:

$$
\begin{aligned}
n_1 \cdot n_2 &= (1)(1) + (1)(-1) + (1)(0) \\
              &= 1 - 1 + 0 \\
              &= 0
\end{aligned}
$$

$$
\|n_1\| = \sqrt{1^2 + 1^2 + 1^2} = \sqrt{3}, \qquad \|n_2\| = \sqrt{1^2 + (-1)^2 + 0^2} = \sqrt{2}
$$

Substituting into the cosine formula:

$$
\cos\theta = \frac{|0|}{\sqrt{3}\sqrt{2}} = 0
$$

Therefore, the angle between the planes is

$$
\theta = \arccos(0) = 90^\circ = \frac{\pi}{2}.
$$

The two planes are perpendicular (orthogonal) to each other.

**3. Why Normal Vectors Alone Are Enough**
A plane is completely determined in orientation by its normal vector, which is perpendicular to every direction within the plane. Rotating a plane in space rotates its normal vector by the exact same angle. Consequently, the dihedral angle formed where two planes meet is identical to the angle formed between their perpendicular normal vectors, making it unnecessary to find their line of intersection first.
