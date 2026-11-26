 
### Exercise 12. A Normal Vector to a Plane

Given the points

$$
A=(1,0,2),\quad B=(2,1,0),\quad C=(0,3,1)
$$

**1. Constructing two vectors in the plane**

The vectors are obtained by subtracting the coordinates of point $A$ from the coordinates of points $B$ and $C$.

$$
\begin{aligned}
\overrightarrow{AB} &= B-A \\
&= (2-1,1-0,0-2) \\
&= (1,1,-2)
\end{aligned}
$$

$$
\begin{aligned}
\overrightarrow{AC} &= C-A \\
&= (0-1,3-0,1-2) \\
&= (-1,3,-1)
\end{aligned}
$$

**2. Finding a normal vector**

A normal vector is perpendicular to both vectors lying in the plane. It can be found using the cross product.

$$
\begin{aligned}
n &= \overrightarrow{AB}\times\overrightarrow{AC} \\
&= (1\cdot(-1)-(-2)\cdot 3, \\
&\quad (-2)\cdot(-1)-1\cdot(-1), \\
&\quad 1\cdot 3-1\cdot(-1)) \\
&= (-1+6,2+1,3+1) \\
&= (5,3,4)
\end{aligned}
$$

Therefore, a normal vector to the plane is

$$
n=(5,3,4)
$$

**3. Verifying perpendicularity**

To verify that $n$ is perpendicular to both vectors, their dot products must be equal to zero.

First, check the dot product with $\overrightarrow{AB}$.

$$
\begin{aligned}
n\cdot\overrightarrow{AB}
&= (5,3,4)\cdot(1,1,-2) \\
&= 5+3-8 \\
&= 0
\end{aligned}
$$

Next, check the dot product with $\overrightarrow{AC}$.

$$
\begin{aligned}
n\cdot\overrightarrow{AC}
&= (5,3,4)\cdot(-1,3,-1) \\
&= -5+9-4 \\
&= 0
\end{aligned}
$$

Both dot products are zero, so the normal vector is perpendicular to both vectors in the plane.

Therefore, $n=(5,3,4)$ is a valid normal vector to the plane determined by the points $A$, $B$, and $C$.

