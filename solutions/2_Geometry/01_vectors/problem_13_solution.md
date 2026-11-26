 
### Exercise 13. Do Four Points Lie in One Plane?

Given the points

$$
A=(0,0,0),\quad B=(1,2,0)
$$

$$
C=(0,1,1),\quad D=(2,5,1)
$$

**1. Constructing the vectors**

The vectors are obtained by subtracting the coordinates of point $A$ from the coordinates of points $B$ and $C$.

$$
\begin{aligned}
\overrightarrow{AB} &= B-A \\
&= (1-0,2-0,0-0) \\
&= (1,2,0)
\end{aligned}
$$

$$
\begin{aligned}
\overrightarrow{AC} &= C-A \\
&= (0-0,1-0,1-0) \\
&= (0,1,1)
\end{aligned}
$$

**2. Finding the normal vector**

The normal vector is obtained by calculating the cross product of the two vectors.

$$
\begin{aligned}
n &= \overrightarrow{AB}\times\overrightarrow{AC} \\
&= (2\cdot 1-0\cdot 1, \\
&\quad 0\cdot 0-1\cdot 1, \\
&\quad 1\cdot 1-2\cdot 0) \\
&= (2,-1,1)
\end{aligned}
$$

Therefore,

$$
n=(2,-1,1)
$$

**3. Constructing $\overrightarrow{AD}$ and checking the dot product**

First, construct the vector from point $A$ to point $D$.

$$
\begin{aligned}
\overrightarrow{AD} &= D-A \\
&= (2-0,5-0,1-0) \\
&= (2,5,1)
\end{aligned}
$$

Now calculate its dot product with the normal vector.

$$
\begin{aligned}
\overrightarrow{AD}\cdot n
&= (2,5,1)\cdot(2,-1,1) \\
&= 2\cdot 2+5\cdot(-1)+1\cdot 1 \\
&= 4-5+1 \\
&= 0
\end{aligned}
$$

**4. Determining coplanarity**

A point $D$ lies in the plane determined by $A$, $B$, and $C$ if the vector $\overrightarrow{AD}$ is perpendicular to the normal vector $n$.

This condition is satisfied when

$$
\overrightarrow{AD}\cdot n=0
$$

Since the calculated dot product is zero, point $D$ lies in the plane determined by points $A$, $B$, and $C$.

Therefore, all four points are coplanar.
   
