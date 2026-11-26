### Exercise 8. Intersection Point of a Line and a Plane

#### Question
Find the intersection point of

$$
(x,y,z)=(1,0,2)+t(1,2,-1)
$$

with the plane $x+y+z=4$. Check the result by substituting it into both descriptions.

#### Solution
Given line and plane are

$$
L: (x, y, z) = (1, 0, 2) + t(1, 2, -1), \qquad \Pi: x + y + z = 4.
$$

**1. Parametric Coordinates of the Line**
Writing the equation of $L$ componentwise gives

$$
\begin{cases}
x = 1 + t, \\
y = 2t, \\
z = 2 - t.
\end{cases}
$$

**2. Finding the Parameter $t$ at the Intersection**
Substituting $x, y, z$ into the plane equation $x + y + z = 4$:

$$
\begin{aligned}
(1 + t) + (2t) + (2 - t) &= 4 \\
3 + 2t &= 4 \\
2t &= 1 \\
t &= \frac{1}{2}
\end{aligned}
$$

**3. Coordinates of the Intersection Point**
Substituting $t = \frac{1}{2}$ back into the parametric equations of $L$:

$$
\begin{aligned}
x &= 1 + \frac{1}{2} = \frac{3}{2} \\
y &= 2\left(\frac{1}{2}\right) = 1 \\
z &= 2 - \frac{1}{2} = \frac{3}{2}
\end{aligned}
$$

Thus, the intersection point is

$$
P = \left(\frac{3}{2}, 1, \frac{3}{2}\right).
$$

**4. Verification in Both Descriptions**
* **In the plane equation ($x + y + z = 4$):**

$$
\frac{3}{2} + 1 + \frac{3}{2} = \frac{6}{2} + 1 = 3 + 1 = 4 \quad (\text{Holds})
$$

* **In the line equation:** For $t = \frac{1}{2}$,

$$
\begin{aligned}
(1, 0, 2) + \frac{1}{2}(1, 2, -1) &= \left(1 + \frac{1}{2},\; 0 + 1,\; 2 - \frac{1}{2}\right) \\
                                  &= \left(\frac{3}{2}, 1, \frac{3}{2}\right) \quad (\text{Holds})
\end{aligned}
$$

Both descriptions are satisfied at $P = \left(\frac{3}{2}, 1, \frac{3}{2}\right)$.
