### Exercise 4. Plane Through Three Points

#### Question
Find the equation of the plane through

$$
A=(1,0,0),\quad B=(0,1,0),\quad C=(0,0,1).
$$

First construct two vectors lying in the plane, and then use the cross product. Check the resulting equation on all three points.

#### Solution
Given points are

$$
A = (1, 0, 0), \qquad B = (0, 1, 0), \qquad C = (0, 0, 1).
$$

**1. Constructing Two Vectors Lying in the Plane**

$$
\begin{aligned}
\overrightarrow{AB} &= B - A \\
                    &= (0 - 1, 1 - 0, 0 - 0) \\
                    &= (-1, 1, 0)
\end{aligned}
$$

$$
\begin{aligned}
\overrightarrow{AC} &= C - A \\
                    &= (0 - 1, 0 - 0, 1 - 0) \\
                    &= (-1, 0, 1)
\end{aligned}
$$

**2. Finding a Normal Vector via Cross Product**
Computing $n = \overrightarrow{AB} \times \overrightarrow{AC}$:

$$
\begin{aligned}
n &= ((1)(1) - (0)(0),\; (0)(-1) - (-1)(1),\; (-1)(0) - (1)(-1)) \\
  &= (1 - 0,\; 0 + 1,\; 0 + 1) \\
  &= (1, 1, 1)
\end{aligned}
$$

**3. Equation of the Plane**
Using point $A = (1, 0, 0)$ and normal vector $n = (1, 1, 1)$ in $n \cdot (X - A) = 0$:

$$
\begin{aligned}
1(x - 1) + 1(y - 0) + 1(z - 0) &= 0 \\
x - 1 + y + z &= 0 \\
x + y + z &= 1
\end{aligned}
$$

**4. Verification on All Three Points**
* **Point $A = (1, 0, 0)$:** $1 + 0 + 0 = 1$ (Holds)
* **Point $B = (0, 1, 0)$:** $0 + 1 + 0 = 1$ (Holds)
* **Point $C = (0, 0, 1)$:** $0 + 0 + 1 = 1$ (Holds)

All three points satisfy the plane equation $x + y + z = 1$.
