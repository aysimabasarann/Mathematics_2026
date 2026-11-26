### Exercise 2. A Line in Space

#### Question
Given

$$
L:(x,y,z)=(2,-1,3)+t(1,2,-2).
$$

State a point on the line and its direction vector, check whether $P=(4,3,-1)$ lies on $L$, and find the point corresponding to $t=-1$.

#### Solution
The given line is

$$
L: (x, y, z) = (2, -1, 3) + t(1, 2, -2), \qquad t \in \mathbb{R}.
$$

**1. Point on the Line and Direction Vector**
Comparing with the standard vector form $(x, y, z) = p_0 + t v$:
* **A point on the line** (corresponding to $t = 0$) is $P_0 = (2, -1, 3)$.
* **A direction vector** of the line is $v = (1, 2, -2)$.

**2. Checking Whether $P = (4, 3, -1)$ Lies on $L$**
Point $P$ lies on $L$ if and only if there exists a single real number $t$ satisfying all three component equations simultaneously:

$$
\begin{cases}
4 = 2 + t, \\
3 = -1 + 2t, \\
-1 = 3 - 2t.
\end{cases}
$$

Solving each equation for $t$:
* From the first equation: $t = 4 - 2 = 2$.
* From the second equation: $2t = 4 \implies t = 2$.
* From the third equation: $-2t = -4 \implies t = 2$.

Since all three equations yield the exact same parameter value $t = 2$, point $P = (4, 3, -1)$ **lies on** the line $L$.

**3. Finding the Point Corresponding to $t = -1$**
Substituting $t = -1$ into the equation of $L$:

$$
\begin{aligned}
(x, y, z) &= (2, -1, 3) + (-1)(1, 2, -2) \\
          &= (2 - 1, -1 - 2, 3 + 2) \\
          &= (1, -3, 5)
\end{aligned}
$$

The point on $L$ corresponding to $t = -1$ is $(1, -3, 5)$.
