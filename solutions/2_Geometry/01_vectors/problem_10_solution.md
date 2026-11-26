 
### Exercise 10. Triangle Area from Vectors

Given the points

$$
A=(0,0,0),\quad B=(2,1,0),\quad C=(1,3,2)
$$

**1. Constructing the vectors**

The vectors are obtained by subtracting the coordinates of point $A$ from the coordinates of points $B$ and $C$.

$$
\begin{aligned}
\overrightarrow{AB} &= B-A \\
&= (2-0,1-0,0-0) \\
&= (2,1,0)
\end{aligned}
$$

$$
\begin{aligned}
\overrightarrow{AC} &= C-A \\
&= (1-0,3-0,2-0) \\
&= (1,3,2)
\end{aligned}
$$

**2. Computing the area of the parallelogram**

The area of a parallelogram formed by two vectors is equal to the length of their cross product.

First, calculate the cross product.

$$
\begin{aligned}
\overrightarrow{AB}\times\overrightarrow{AC}
&= (1\cdot 2-0\cdot 3, \\
&\quad 0\cdot 1-2\cdot 2, \\
&\quad 2\cdot 3-1\cdot 1) \\
&= (2,-4,5)
\end{aligned}
$$

Now calculate its length.

$$
\begin{aligned}
\|\overrightarrow{AB}\times\overrightarrow{AC}\|
&= \sqrt{2^2+(-4)^2+5^2} \\
&= \sqrt{4+16+25} \\
&= \sqrt{45} \\
&= 3\sqrt{5}
\end{aligned}
$$

Therefore, the area of the parallelogram is

$$
A_{\mathrm{parallelogram}}=3\sqrt{5}
$$

**3. Computing the area of the triangle**

The area of a triangle formed by two vectors is half the area of the parallelogram formed by the same vectors.

$$
\begin{aligned}
A_{\mathrm{triangle}}
&= \frac{1}{2}\|\overrightarrow{AB}\times\overrightarrow{AC}\| \\
&= \frac{1}{2}(3\sqrt{5}) \\
&= \frac{3\sqrt{5}}{2}
\end{aligned}
$$

**4. Geometric interpretation**

The two vectors form a parallelogram, whose area is given by the magnitude of their cross product. A diagonal divides a parallelogram into two congruent triangles. Therefore, the area of the triangle is half the area of the parallelogram.

The factor $\frac{1}{2}$ represents this geometric relationship.
 
