### Exercise 11. Plane Containing a Line and a Point

#### Question
Find the equation of the plane containing

$$
(x,y,z)=(1,0,2)+t(1,1,-1)
$$

and the point $P=(0,2,1)$. Check that both the entire line and the point lie in the plane you obtain.

#### Solution
Given line and external point are

$$
L: (x, y, z) = (1, 0, 2) + t(1, 1, -1), \qquad P = (0, 2, 1).
$$

**1. Constructing Two Direction Vectors in the Plane**
From the equation of $L$, we extract a point on the line $P_0 = (1, 0, 2)$ and its direction vector $v_1 = (1, 1, -1)$. A second vector lying in the plane is obtained by connecting $P_0$ to $P$:

$$
\begin{aligned}
v_2 &= \overrightarrow{P_0 P} \\
    &= P - P_0 \\
    &= (0 - 1, 2 - 0, 1 - 2) \\
    &= (-1, 2, -1)
\end{aligned}
$$

**2. Finding a Normal Vector to the Plane**
Taking the cross product $n = v_1 \times v_2$ gives a vector perpendicular to both directions in the plane:

$$
\begin{aligned}
n &= ((1)(-1) - (-1)(2),\; (-1)(-1) - (1)(-1),\; (1)(2) - (1)(-1)) \\
  &= (-1 + 2,\; 1 + 1,\; 2 + 1) \\
  &= (1, 2, 3)
\end{aligned}
$$

**3. Equation of the Plane**
Using point $P_0 = (1, 0, 2)$ and normal vector $n = (1, 2, 3)$ in $n \cdot (X - P_0) = 0$:

$$
\begin{aligned}
1(x - 1) + 2(y - 0) + 3(z - 2) &= 0 \\
x - 1 + 2y + 3z - 6 &= 0 \\
x + 2y + 3z &= 7
\end{aligned}
$$

**4. Verification**
* **Point $P = (0, 2, 1)$:** Substituting into $x + 2y + 3z = 7$:

$$
0 + 2(2) + 3(1) = 0 + 4 + 3 = 7
$$

* **The entire line $L$:** Substituting an arbitrary point $(x, y, z) = (1 + t,\; t,\; 2 - t)$ from $L$ for any $t \in \mathbb{R}$:

$$
\begin{aligned}
(1 + t) + 2(t) + 3(2 - t) &= 1 + t + 2t + 6 - 3t \\
                           &= (1 + 6) + (1 + 2 - 3)t \\
                           &= 7 + 0 \\
                           &= 7
\end{aligned}
$$

Since the identity holds for every $t \in \mathbb{R}$ and also at $P$, both the entire line $L$ and the point $P$ lie in the plane $x + 2y + 3z = 7$.
