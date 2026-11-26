
### Exercise 9. Cross Product as a Perpendicular Direction

Given the vectors

$$
u=(1,2,0),\qquad v=(0,1,3)
$$

**1. Computing the cross product**

The cross product in $\mathbb R^3$ is calculated using the determinant formula.

$$
u\times v=
\begin{pmatrix}
2\cdot 3-0\cdot 1, \\
0\cdot 0-1\cdot 3, \\
1\cdot 1-2\cdot 0
\end{pmatrix}
$$

Therefore,

$$
u\times v=(6,-3,1)
$$

**2. Verifying perpendicularity**

The cross product must be perpendicular to both original vectors. This can be checked using dot products.

First, check perpendicularity to $u$.

$$
\begin{aligned}
(u\times v)\cdot u &= (6,-3,1)\cdot(1,2,0) \\
&= 6-6+0 \\
&= 0
\end{aligned}
$$

Next, check perpendicularity to $v$.

$$
\begin{aligned}
(u\times v)\cdot v &= (6,-3,1)\cdot(0,1,3) \\
&= 0-3+3 \\
&= 0
\end{aligned}
$$

Therefore, $u\times v$ is perpendicular to both $u$ and $v$.

**3. Computing the cross product in the reverse order**

Using the same formula with the order of the vectors reversed:

$$
v\times u=(-6,3,-1)
$$

**4. Comparing the results**

Comparing the two cross products:

$$
\begin{aligned}
v\times u &= (-6,3,-1) \\
&= -(6,-3,1) \\
&= -(u\times v)
\end{aligned}
$$

Therefore, reversing the order of the vectors changes the sign of the cross product but preserves its magnitude.

This shows that the cross product is anti-commutative.

