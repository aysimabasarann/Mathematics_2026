 ### Exercise 13. Do Four Points Lie in One Plane?

#### Question
Given

$$
A=(0,0,0),\qquad B=(1,2,0),\qquad C=(0,1,1),\qquad D=(2,5,1).
$$

1. Construct $\overrightarrow{AB}$ and $\overrightarrow{AC}$.
2. Find $n=\overrightarrow{AB}\times\overrightarrow{AC}$.
3. Construct $\overrightarrow{AD}$ and check whether $\overrightarrow{AD}\cdot n=0$.
4. Based on this, decide whether $D$ lies in the plane determined by $A,B,C$, and justify the criterion.

#### Solution
Given points are

$$
A = (0, 0, 0), \qquad B = (1, 2, 0), \qquad C = (0, 1, 1), \qquad D = (2, 5, 1).
$$

**1. Construction of $\overrightarrow{AB}$ and $\overrightarrow{AC}$**

$$
\begin{aligned}
\overrightarrow{AB} &= B - A \\
                    &= (1 - 0, 2 - 0, 0 - 0) \\
                    &= (1, 2, 0)
\end{aligned}
$$

$$
\begin{aligned}
\overrightarrow{AC} &= C - A \\
                    &= (0 - 0, 1 - 0, 1 - 0) \\
                    &= (0, 1, 1)
\end{aligned}
$$

**2. Finding the Normal Vector $n$**

$$
\begin{aligned}
n &= \overrightarrow{AB} \times \overrightarrow{AC} \\
  &= ((2)(1) - (0)(1),\; (0)(0) - (1)(1),\; (1)(1) - (2)(0)) \\
  &= (2 - 0,\; 0 - 1,\; 1 - 0) \\
  &= (2, -1, 1)
\end{aligned}
$$

**3. Construction of $\overrightarrow{AD}$ and Dot Product Test**

$$
\begin{aligned}
\overrightarrow{AD} &= D - A \\
                    &= (2 - 0, 5 - 0, 1 - 0) \\
                    &= (2, 5, 1)
\end{aligned}
$$

Computing $\overrightarrow{AD} \cdot n$:

$$
\begin{aligned}
\overrightarrow{AD} \cdot n &= (2)(2) + (5)(-1) + (1)(1) \\
                            &= 4 - 5 + 1 \\
                            &= 0
\end{aligned}
$$

**4. Decision and Justification**
Yes, point $D$ **lies in the plane** determined by $A$, $B$, and $C$. The vector $n = \overrightarrow{AB} \times \overrightarrow{AC}$ is perpendicular to the plane spanned by $A$, $B$, and $C$. Since $\overrightarrow{AD} \cdot n = 0$, the vector $\overrightarrow{AD}$ is orthogonal to this normal vector, which means $\overrightarrow{AD}$ lies entirely inside the plane and therefore $A, B, C, D$ are coplanar.



 
