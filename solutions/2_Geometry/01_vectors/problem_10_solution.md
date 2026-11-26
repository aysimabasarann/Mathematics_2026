 ### Exercise 10. Triangle Area from Vectors

#### Question
The points $A=(0,0,0)$, $B=(2,1,0)$, and $C=(1,3,2)$ form a triangle. Construct $\overrightarrow{AB}$ and $\overrightarrow{AC}$, compute the area of the parallelogram using the cross product, and then find the area of the triangle. Explain the factor $\frac12$.

#### Solution
Given points are

$$
A = (0, 0, 0), \qquad B = (2, 1, 0), \qquad C = (1, 3, 2).
$$

**1. Construction of $\overrightarrow{AB}$ and $\overrightarrow{AC}$**

$$
\begin{aligned}
\overrightarrow{AB} &= B - A \\
                    &= (2 - 0, 1 - 0, 0 - 0) \\
                    &= (2, 1, 0)
\end{aligned}
$$

$$
\begin{aligned}
\overrightarrow{AC} &= C - A \\
                    &= (1 - 0, 3 - 0, 2 - 0) \\
                    &= (1, 3, 2)
\end{aligned}
$$

**2. Area of the Parallelogram**
First, compute the cross product $\overrightarrow{AB} \times \overrightarrow{AC}$:

$$
\begin{aligned}
\overrightarrow{AB} \times \overrightarrow{AC} &= ((1)(2) - (0)(3),\; (0)(1) - (2)(2),\; (2)(3) - (1)(1)) \\
                                                  &= (2 - 0,\; 0 - 4,\; 6 - 1) \\
                                                  &= (2, -4, 5)
\end{aligned}
$$

The area of the parallelogram spanned by $\overrightarrow{AB}$ and $\overrightarrow{AC}$ equals the length of their cross product:

$$
\begin{aligned}
A_{\mathrm{parallelogram}} &= \|\overrightarrow{AB} \times \overrightarrow{AC}\| \\
                           &= \sqrt{2^2 + (-4)^2 + 5^2} \\
                           &= \sqrt{4 + 16 + 25} \\
                           &= \sqrt{45} \\
                           &= 3\sqrt{5}
\end{aligned}
$$

**3. Area of the Triangle**

$$
\begin{aligned}
A_{\mathrm{triangle}} &= \frac{1}{2} \|\overrightarrow{AB} \times \overrightarrow{AC}\| \\
                        &= \frac{1}{2} (3\sqrt{5}) \\
                        &= \frac{3\sqrt{5}}{2}
\end{aligned}
$$

**4. Explanation of the Factor $\frac{1}{2}$**
Any parallelogram spanned by two adjacent vectors $\overrightarrow{AB}$ and $\overrightarrow{AC}$ is divided by its diagonal $BC$ into two congruent triangles of equal area. Therefore, the area of $\triangle ABC$ is exactly half the area of the full parallelogram.

