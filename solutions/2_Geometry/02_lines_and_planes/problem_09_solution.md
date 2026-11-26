### Exercise 9. Distances

#### Question
Compute:

1. the distance from $P=(2,3)$ to the line $3x+4y-10=0$,
2. the distance from $Q=(2,-1,3)$ to the plane $2x-2y+z-4=0$.

Compare the two formulas and explain their common connection with the normal direction.

#### Solution

**1. Distance from Point to Line in $\mathbb{R}^2$**
The distance $d$ from a point $(x_0, y_0) = (2, 3)$ to the line given by $ax + by + c = 0$ ($3x + 4y - 10 = 0$) is computed using the formula:

$$
d = \frac{|ax_0 + by_0 + c|}{\sqrt{a^2 + b^2}}
$$

Substituting the values:

$$
\begin{aligned}
d &= \frac{|3(2) + 4(3) - 10|}{\sqrt{3^2 + 4^2}} \\
  &= \frac{|6 + 12 - 10|}{\sqrt{9 + 16}} \\
  &= \frac{|8|}{\sqrt{25}} \\
  &= \frac{8}{5}
\end{aligned}
$$

**2. Distance from Point to Plane in $\mathbb{R}^3$**
The distance $d$ from a point $(x_0, y_0, z_0) = (2, -1, 3)$ to the plane given by $ax + by + cz + d = 0$ ($2x - 2y + z - 4 = 0$) is computed using the formula:

$$
d = \frac{|ax_0 + by_0 + cz_0 + d|}{\sqrt{a^2 + b^2 + c^2}}
$$

Substituting the values:

$$
\begin{aligned}
d &= \frac{|2(2) - 2(-1) + 1(3) - 4|}{\sqrt{2^2 + (-2)^2 + 1^2}} \\
  &= \frac{|4 + 2 + 3 - 4|}{\sqrt{4 + 4 + 1}} \\
  &= \frac{|5|}{\sqrt{9}} \\
  &= \frac{5}{3}
\end{aligned}
$$

**3. Comparison and Connection with the Normal Direction**
Both formulas share the exact same geometric and algebraic structure: the numerator evaluates how much the given point fails to satisfy the equation of the object, while the denominator divides by the magnitude of the normal vector ($(a, b)$ for the line, $(a, b, c)$ for the plane). Geometrically, both compute the length of the orthogonal projection along the normal direction.
