### Exercise 14. Contrast: Intersection and Parallelism

#### Question
From the point $P=(0,0,1)$, two lines are drawn with direction vectors

$$
v_1=(2,1,-1),\qquad v_2=(2,1,0).
$$

For each line, analyze its position relative to the plane $z=0$.

For the line that intersects the plane, find the intersection point. For the other line, explain how you can recognize parallelism without solving an equation.

#### Solution
Given point is $P = (0, 0, 1)$ and the plane is $\Pi: z = 0$ (the $xy$-plane), whose normal vector is $n = (0, 0, 1)$.

**1. Analysis of Line $L_1$ (Direction $v_1 = (2, 1, -1)$)**
The parametric equation of $L_1$ is

$$
\begin{cases}
x = 2t, \\
y = t, \\
z = 1 - t.
\end{cases}
$$

Substituting the $z$-coordinate into the plane equation $z = 0$:

$$
1 - t = 0 \implies t = 1
$$

Since a unique parameter value $t = 1$ exists, $L_1$ intersects the plane at a single point. Substituting $t = 1$ into the parametric equations gives the intersection point:

$$
(2(1), 1, 1 - 1) = (2, 1, 0).
$$

**2. Analysis of Line $L_2$ (Direction $v_2 = (2, 1, 0)$)**
The parametric equation of $L_2$ is

$$
\begin{cases}
x = 2s, \\
y = s, \\
z = 1.
\end{cases}
$$

Substituting the $z$-coordinate into the plane equation $z = 0$:

$$
1 = 0
$$

This yields a contradiction, meaning $L_2$ has no points in common with the plane and is therefore parallel to it.

**3. Recognizing Parallelism Without Solving an Equation**
We can determine that $L_2$ is parallel to the plane by computing the dot product of its direction vector $v_2 = (2, 1, 0)$ with the plane's normal vector $n = (0, 0, 1)$:

$$
v_2 \cdot n = (2)(0) + (1)(0) + (0)(1) = 0.
$$

Since the dot product is zero, the direction vector is orthogonal to the normal vector, meaning the line runs parallel to the plane. Furthermore, because the starting point $P = (0, 0, 1)$ does not satisfy $z = 0$, the line is strictly parallel with no intersection.
