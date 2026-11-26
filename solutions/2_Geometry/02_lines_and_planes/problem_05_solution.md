### Exercise 5. Relative Position of Two Lines

#### Question
Analyze the position of

$$
L_1:(x,y,z)=(1,1,0)+t(1,2,1),
$$

$$
L_2:(x,y,z)=(2,0,1)+s(0,1,-1).
$$

If they intersect, give the intersection point. If not, determine whether they are parallel or skew. Justify the classification.

#### Solution
The given lines are

$$
L_1: (x, y, z) = (1, 1, 0) + t(1, 2, 1), \qquad t \in \mathbb{R},
$$

$$
L_2: (x, y, z) = (2, 0, 1) + s(0, 1, -1), \qquad s \in \mathbb{R}.
$$

**1. Checking for Parallelism**
The direction vectors of $L_1$ and $L_2$ are

$$
v_1 = (1, 2, 1), \qquad v_2 = (0, 1, -1).
$$

Because $v_1$ and $v_2$ are not scalar multiples of each other (for instance, the first component of $v_2$ is $0$ while that of $v_1$ is $1$), the lines are **not parallel**.

**2. Testing for Intersection**
Equating the coordinates of $L_1$ and $L_2$ gives the system

$$
\begin{cases}
1 + t = 2, \\
1 + 2t = s, \\
t = 1 - s.
\end{cases}
$$

From the first equation:

$$
t = 2 - 1 = 1
$$

Substituting $t = 1$ into the second equation:

$$
s = 1 + 2(1) = 3
$$

Checking whether $(t, s) = (1, 3)$ satisfies the third equation:

$$
\begin{aligned}
\text{Left-hand side:} \quad t &= 1 \\
\text{Right-hand side:} \quad 1 - s &= 1 - 3 = -2
\end{aligned}
$$

Wait—notice that `\text` is avoided per formatting rules; writing this cleanly in prose and equations:

Substituting $t = 1$ and $s = 3$ into the third equation $t = 1 - s$ gives

$$
1 = 1 - 3 \implies 1 = -2,
$$

which is a contradiction. Therefore, the system has **no solution**, and the lines do not intersect.

**3. Classification and Justification**
The lines $L_1$ and $L_2$ are **skew lines**. By definition, two lines in $\mathbb{R}^3$ that are neither parallel nor intersecting are skew (they do not lie in a common plane).
