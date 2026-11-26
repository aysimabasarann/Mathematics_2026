 
### Exercise 6. Projection and Perpendicular Component

Given the vectors

$$
u=(4,2),\qquad v=(1,1)
$$

**1. Computing the projection of $u$ onto $v$**

The projection of a vector $u$ onto a nonzero vector $v$ is calculated using the formula

$$
\mathrm{proj}_v\,u=\frac{u\cdot v}{v\cdot v}v
$$

First, calculate the dot product.

$$
\begin{aligned}
u\cdot v &= 4\cdot 1+2\cdot 1 \\
&= 6
\end{aligned}
$$

Calculate the squared length of $v$.

$$
\begin{aligned}
v\cdot v &= 1^2+1^2 \\
&= 2
\end{aligned}
$$

Substitute these values into the projection formula.

$$
\begin{aligned}
\mathrm{proj}_v\,u &= \frac{6}{2}(1,1) \\
&= 3(1,1) \\
&= (3,3)
\end{aligned}
$$

**2. Computing the perpendicular component**

The perpendicular component is obtained by subtracting the projection from the original vector.

$$
\begin{aligned}
r &= u-\mathrm{proj}_v\,u \\
&= (4,2)-(3,3) \\
&= (1,-1)
\end{aligned}
$$

**3. Verification of perpendicularity**

Two vectors are perpendicular if their dot product is zero.

$$
\begin{aligned}
r\cdot v &= (1,-1)\cdot(1,1) \\
&= 1\cdot 1+(-1)\cdot 1 \\
&= 1-1 \\
&= 0
\end{aligned}
$$

Therefore, $r$ is perpendicular to $v$.

**4. Geometric interpretation**

The projection $(3,3)$ represents the component of $u$ parallel to the direction of $v$. The vector $r=(1,-1)$ represents the remaining component, which is perpendicular to $v$.

Thus, the original vector is decomposed into two perpendicular components: one parallel to $v$ and one perpendicular to $v$.

