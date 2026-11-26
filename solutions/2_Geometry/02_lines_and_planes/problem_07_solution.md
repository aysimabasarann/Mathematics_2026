### Exercise 7. A Line Relative to a Plane

#### Question
For

$$
L:(x,y,z)=(1,1,0)+t(1,-1,0),\qquad \Pi:x+y+z=2,
$$

determine whether the line intersects the plane at one point, is parallel to it, or lies in it. Explain the role of the dot product of the direction vector and the normal vector.

#### Solution
Given line and plane are

$$
L: (x, y, z) = (1, 1, 0) + t(1, -1, 0), \qquad \Pi: x + y + z = 2.
$$

**1. Extracting Direction and Normal Vectors**
From the equation of $L$, a point on the line is $P_0 = (1, 1, 0)$ and its direction vector is

$$
v = (1, -1, 0).
$$

From the equation of $\Pi$, a normal vector to the plane is

$$
n = (1, 1, 1).
$$

**2. Checking the Dot Product $v \cdot n$**

$$
\begin{aligned}
v \cdot n &= (1)(1) + (-1)(1) + (0)(1) \\
          &= 1 - 1 + 0 \\
          &= 0
\end{aligned}
$$

Since $v \cdot n = 0$, the direction vector $v$ is perpendicular to the normal vector $n$, meaning the line $L$ is parallel to the plane $\Pi$ (either strictly parallel with no intersection, or entirely contained in $\Pi$).

**3. Testing Whether $P_0 = (1, 1, 0)$ Lies in $\Pi$**
Substituting the point $P_0 = (1, 1, 0)$ into the plane equation $x + y + z = 2$:

$$
\begin{aligned}
1 + 1 + 0 &= 2 \\
2 &= 2
\end{aligned}
$$

Since $P_0$ satisfies the plane equation (and for any $t \in \mathbb{R}$, $(1 + t) + (1 - t) + 0 = 2$), every point of $L$ lies in $\Pi$. Thus, the line $L$ **lies in** the plane $\Pi$.

**4. Role of the Dot Product $v \cdot n$**
The normal vector $n$ is perpendicular to the plane $\Pi$. Therefore, the dot product $v \cdot n$ tests whether the line's direction $v$ is parallel to the plane:
* If $v \cdot n \neq 0$, the line is not parallel to the plane and must intersect it at a single unique point.
* If $v \cdot n = 0$, the line runs parallel to the plane, reducing the problem to checking a single point of the line to distinguish between being strictly parallel ($0$ common points) and lying inside the plane (infinitely many common points).
