### Exercise 1. Line Through Two Points

#### Question
Find the equation of the line through $A=(1,2)$ and $B=(4,-1)$ in parametric and general form. Identify a direction vector and an example of a normal vector. Check that both points satisfy the equation you obtain.

#### Solution
Given points are

$$
A = (1, 2), \qquad B = (4, -1).
$$

**1. Direction Vector**
A direction vector $v$ for the line is given by the displacement vector from $A$ to $B$:

$$
\begin{aligned}
v &= \overrightarrow{AB} \\
  &= B - A \\
  &= (4 - 1, -1 - 2) \\
  &= (3, -3)
\end{aligned}
$$

(Any nonzero scalar multiple, such as $(1, -1)$, is also a valid direction vector.)

**2. Parametric Form**
Using the point $A = (1, 2)$ and direction vector $v = (3, -3)$, the parametric equation of the line is

$$
(x, y) = (1, 2) + t(3, -3), \qquad t \in \mathbb{R},
$$

or componentwise:

$$
\begin{cases}
x = 1 + 3t, \\
y = 2 - 3t.
\end{cases}
$$

**3. General Form and Normal Vector**
Eliminating the parameter $t$ by adding the two parametric equations gives

$$
\begin{aligned}
x + y &= (1 + 3t) + (2 - 3t) \\
x + y &= 3 \\
x + y - 3 &= 0
\end{aligned}
$$

From the general form $ax + by + c = 0$, the coefficients of $x$ and $y$ directly give a normal vector perpendicular to the line:

$$
n = (1, 1).
$$

We can verify orthogonality with the direction vector: $v \cdot n = (3)(1) + (-3)(1) = 0$.

**4. Verification on Both Points**
* Substituting $A = (1, 2)$ into $x + y - 3 = 0$:

$$
1 + 2 - 3 = 0 \quad (\text{Holds})
$$

* Substituting $B = (4, -1)$ into $x + y - 3 = 0$:

$$
4 + (-1) - 3 = 0 \quad (\text{Holds})
$$

Both points satisfy the general equation (and correspond to $t = 0$ and $t = 1$ in the parametric form).
