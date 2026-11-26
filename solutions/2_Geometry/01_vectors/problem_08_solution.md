
### Exercise 8. Linear Combination and Checking the Result

Given the vectors

$$
w=(5,1),\qquad u=(1,1),\qquad v=(2,-1)
$$

**1. Setting up the linear combination**

We want to determine whether $w$ can be expressed as

$$
w=au+bv
$$

Substituting the given vectors:

$$
\begin{aligned}
(5,1) &= a(1,1)+b(2,-1) \\
&= (a,a)+(2b,-b) \\
&= (a+2b,a-b)
\end{aligned}
$$

Comparing the corresponding components gives the system

$$
\begin{cases}
a+2b=5, \\
a-b=1.
\end{cases}
$$

**2. Finding the coefficients**

From the second equation:

$$
a=1+b
$$

Substitute this expression into the first equation.

$$
\begin{aligned}
1+b+2b &= 5 \\
3b &= 4 \\
b &= \frac{4}{3}
\end{aligned}
$$

Now calculate $a$.

$$
\begin{aligned}
a &= 1+\frac{4}{3} \\
&= \frac{7}{3}
\end{aligned}
$$

Therefore,

$$
a=\frac{7}{3},\qquad b=\frac{4}{3}
$$

**3. Reconstructing and checking the vector**

Substitute the calculated coefficients into the linear combination.

$$
\begin{aligned}
au+bv &= \frac{7}{3}(1,1)+\frac{4}{3}(2,-1) \\
&= \left(\frac{7}{3},\frac{7}{3}\right)
+\left(\frac{8}{3},-\frac{4}{3}\right) \\
&= \left(\frac{15}{3},\frac{3}{3}\right) \\
&= (5,1) \\
&= w
\end{aligned}
$$

Thus, $w$ can be expressed as a linear combination of $u$ and $v$.

**4. Geometric interpretation**

A linear combination represents the addition of scalar multiples of vectors. The coefficients determine how much each vector is scaled and whether its orientation is preserved or reversed.

Since $w$ is obtained from $au+bv$, it lies in the span of $u$ and $v$. In this case, the two vectors span the entire plane.

