### Exercise 8. Linear Combination and Checking the Result

#### Question
Check whether $w=(5,1)$ can be written as

$$
w=au+bv,
$$

where $u=(1,1)$ and $v=(2,-1)$. If so, find $a,b$, reconstruct $w$ from them, and explain the geometric meaning of the existence of such coefficients.

#### Solution
Given vectors are

$$
w = (5, 1), \qquad u = (1, 1), \qquad v = (2, -1).
$$

**1. Setting Up the Linear System**
Writing $w = au + bv$ in coordinate form gives

$$
\begin{aligned}
a(1, 1) + b(2, -1) &= (5, 1) \\
(a + 2b, a - b) &= (5, 1)
\end{aligned}
$$

Equating components yields the system of linear equations

$$
\begin{cases}
a + 2b = 5, \\
a - b = 1.
\end{cases}
$$

**2. Solving for $a$ and $b$**
Subtracting the second equation from the first eliminates $a$:

$$
\begin{aligned}
(a + 2b) - (a - b) &= 5 - 1 \\
3b &= 4 \\
b &= \frac{4}{3}
\end{aligned}
$$

Substituting $b = \frac{4}{3}$ into $a - b = 1$:

$$
\begin{aligned}
a - \frac{4}{3} &= 1 \\
a &= 1 + \frac{4}{3} \\
a &= \frac{7}{3}
\end{aligned}
$$

Thus, $w$ can be written as a linear combination of $u$ and $v$ with $a = \frac{7}{3}$ and $b = \frac{4}{3}$.

**3. Reconstruction of $w$**

$$
\begin{aligned}
au + bv &= \frac{7}{3}(1, 1) + \frac{4}{3}(2, -1) \\
        &= \left(\frac{7}{3}, \frac{7}{3}\right) + \left(\frac{8}{3}, -\frac{4}{3}\right) \\
        &= \left(\frac{7 + 8}{3}, \frac{7 - 4}{3}\right) \\
        &= \left(\frac{15}{3}, \frac{3}{3}\right) \\
        &= (5, 1) \\
        &= w
\end{aligned}
$$

**4. Geometric Meaning**
Geometrically, the vectors $u$ and $v$ are not collinear, so they span the entire two-dimensional plane $\mathbb{R}^2$. The existence of unique scalars $a$ and $b$ means that the point $(5, 1)$ can be reached from the origin by moving $\frac{7}{3}$ units along the direction of $u$ and then $\frac{4}{3}$ units along the direction of $v$.

