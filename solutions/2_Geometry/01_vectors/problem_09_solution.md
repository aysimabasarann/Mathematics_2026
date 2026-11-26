### Exercise 9. Cross Product as a Perpendicular Direction

#### Question
For $u=(1,2,0)$ and $v=(0,1,3)$ compute $u\times v$. Use dot products to check perpendicularity to both vectors, compute $v\times u$, and compare the results.

#### Solution
Given vectors are

$$
u = (1, 2, 0), \qquad v = (0, 1, 3).
$$

**1. Computation of $u \times v$**
Using the cross product formula $u \times v = (u_2 v_3 - u_3 v_2,\; u_3 v_1 - u_1 v_3,\; u_1 v_2 - u_2 v_1)$:

$$
\begin{aligned}
u \times v &= ((2)(3) - (0)(1),\; (0)(0) - (1)(3),\; (1)(1) - (2)(0)) \\
           &= (6 - 0,\; 0 - 3,\; 1 - 0) \\
           &= (6, -3, 1)
\end{aligned}
$$

**2. Verification of Perpendicularity**
Checking the dot product of $u \times v$ with $u$:

$$
\begin{aligned}
(u \times v) \cdot u &= (6)(1) + (-3)(2) + (1)(0) \\
                     &= 6 - 6 + 0 \\
                     &= 0
\end{aligned}
$$

Checking the dot product of $u \times v$ with $v$:

$$
\begin{aligned}
(u \times v) \cdot v &= (6)(0) + (-3)(1) + (1)(3) \\
                     &= 0 - 3 + 3 \\
                     &= 0
\end{aligned}
$$

Since both dot products equal zero, $u \times v$ is perpendicular to both $u$ and $v$.

**3. Computation of $v \times u$**
Using the cross product formula $v \times u = (v_2 u_3 - v_3 u_2,\; v_3 u_1 - v_1 u_3,\; v_1 u_2 - v_2 u_1)$:

$$
\begin{aligned}
v \times u &= ((1)(0) - (3)(2),\; (3)(1) - (0)(0),\; (0)(2) - (1)(1)) \\
           &= (0 - 6,\; 3 - 0,\; 0 - 1) \\
           &= (-6, 3, -1)
\end{aligned}
$$

**4. Comparison of Results**
Comparing the two results shows that

$$
v \times u = (-6, 3, -1) = -(6, -3, 1) = -(u \times v).
$$

Reversing the order of the vectors in a cross product preserves the magnitude and perpendicular line of direction, but reverses the orientation (sign) of the resulting vector (anticommutativity).



 
