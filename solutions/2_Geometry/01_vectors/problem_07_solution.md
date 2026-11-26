  
### Exercise 7. Linear Dependence Without Heavy Computation

Given the vectors

$$
u=(1,2,3),\qquad v=(2,4,6),\qquad w=(0,1,1)
$$

**1. Identifying the relation between $u$ and $v$**

Comparing the corresponding components of the vectors, we obtain

$$
\begin{aligned}
v &= (2,4,6) \\
&= 2(1,2,3) \\
&= 2u
\end{aligned}
$$

Therefore, $v=2u$. The vectors $u$ and $v$ are scalar multiples of each other.

**2. Determining linear independence**

A set of vectors is linearly dependent if at least one vector can be expressed as a linear combination of the others.

Since $v=2u$, we can write

$$
2u-v+0w=(0,0,0)
$$

This is a nontrivial linear relation because the coefficients are not all zero.

Therefore, the three vectors are linearly dependent.

**3. Explanation without lengthy computation**

There is no need for a long calculation because the relation $v=2u$ is immediately visible from their coordinates.

Since two of the vectors are already scalar multiples of each other, the set cannot be linearly independent, regardless of the third vector.

