 ### Exercise 6. Projection and Perpendicular Component

#### Question
Find the projection of $u=(4,2)$ onto the direction $v=(1,1)$. Then compute

$$
r=u-\mathrm{proj}_v\,u
$$

and verify that $r\cdot v=0$. Explain this result geometrically.

#### Solution
Given vectors are

$$
u = (4, 2), \qquad v = (1, 1).
$$

**1. Projection of $u$ onto $v$**
The orthogonal projection formula is

$$
\mathrm{proj}_v\,u = \frac{u \cdot v}{v \cdot v} v.
$$

Computing the dot products:

$$
\begin{aligned}
u \cdot v &= (4)(1) + (2)(1) \\
          &= 4 + 2 \\
          &= 6
\end{aligned}
$$

$$
\begin{aligned}
v \cdot v &= (1)(1) + (1)(1) \\
          &= 1 + 1 \\
          &= 2
\end{aligned}
$$

Substituting these values into the projection formula:

$$
\begin{aligned}
\mathrm{proj}_v\,u &= \frac{6}{2}(1, 1) \\
                   &= 3(1, 1) \\
                   &= (3, 3)
\end{aligned}
$$

**2. Computation of the Perpendicular Component $r$**

$$
\begin{aligned}
r &= u - \mathrm{proj}_v\,u \\
  &= (4, 2) - (3, 3) \\
  &= (4 - 3, 2 - 3) \\
  &= (1, -1)
\end{aligned}
$$

**3. Verification that $r \cdot v = 0$**

$$
\begin{aligned}
r \cdot v &= (1)(1) + (-1)(1) \\
          &= 1 - 1 \\
          &= 0
\end{aligned}
$$

Since $r \cdot v = 0$, the vector $r$ is orthogonal (perpendicular) to $v$.

**4. Geometric Explanation**
Geometrically, $\mathrm{proj}_v\,u$ is the shadow of $u$ cast orthogonally onto the line spanned by $v$. Subtracting this parallel component from $u$ leaves the residual vector $r$, which connects the tip of the projection to the tip of $u$ at a right angle. Thus, $u$ is decomposed into two orthogonal vectors: one parallel to $v$ and one perpendicular to $v$.
