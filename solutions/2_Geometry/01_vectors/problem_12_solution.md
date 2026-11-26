 ### Exercise 12. A Normal Vector to a Plane

#### Question
Given $A=(1,0,2)$, $B=(2,1,0)$, and $C=(0,3,1)$. Construct two vectors lying in the plane, find a vector perpendicular to both, and check the perpendicularity using dot products.

#### Solution
Given points are

$$
A = (1, 0, 2), \qquad B = (2, 1, 0), \qquad C = (0, 3, 1).
$$

**1. Constructing Two Vectors Lying in the Plane**

$$
\begin{aligned}
\overrightarrow{AB} &= B - A \\
                    &= (2 - 1, 1 - 0, 0 - 2) \\
                    &= (1, 1, -2)
\end{aligned}
$$

$$
\begin{aligned}
\overrightarrow{AC} &= C - A \\
                    &= (0 - 1, 3 - 0, 1 - 2) \\
                    &= (-1, 3, -1)
\end{aligned}
$$

**2. Finding a Normal Vector Perpendicular to Both**
A vector $n$ perpendicular to both $\overrightarrow{AB}$ and $\overrightarrow{AC}$ is obtained using their cross product:

$$
\begin{aligned}
n &= \overrightarrow{AB} \times \overrightarrow{AC} \\
  &= ((1)(-1) - (-2)(3),\; (-2)(-1) - (1)(-1),\; (1)(3) - (1)(-1)) \\
  &= (-1 + 6,\; 2 + 1,\; 3 + 1) \\
  &= (5, 3, 4)
\end{aligned}
$$

**3. Verification of Perpendicularity Using Dot Products**
Checking the dot product of $n$ with $\overrightarrow{AB}$:

$$
\begin{aligned}
n \cdot \overrightarrow{AB} &= (5)(1) + (3)(1) + (4)(-2) \\
                            &= 5 + 3 - 8 \\
                            &= 0
\end{aligned}
$$

Checking the dot product of $n$ with $\overrightarrow{AC}$:

$$
\begin{aligned}
n \cdot \overrightarrow{AC} &= (5)(-1) + (3)(3) + (4)(-1) \\
                            &= -5 + 9 - 4 \\
                            &= 0
\end{aligned}
$$

Since both dot products equal zero, $n = (5, 3, 4)$ is confirmed to be perpendicular to both vectors and therefore normal to the plane.
 
