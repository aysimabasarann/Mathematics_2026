
### Exercise 11. Decomposition into Parallel and Perpendicular Components

Given the vectors

$$
u=(3,4),\qquad v=(1,2)
$$

**1. Finding the parallel component**

The parallel component of $u$ in the direction of $v$ is calculated using the projection formula.

$$
u_{\parallel}=\frac{u\cdot v}{v\cdot v}v
$$

First, calculate the dot products.

$$
\begin{aligned}
u\cdot v &= 3\cdot 1+4\cdot 2 \\
&= 3+8 \\
&= 11
\end{aligned}
$$

$$
\begin{aligned}
v\cdot v &= 1^2+2^2 \\
&= 1+4 \\
&= 5
\end{aligned}
$$

Substitute these values into the projection formula.

$$
\begin{aligned}
u_{\parallel} &= \frac{11}{5}(1,2) \\
&= \left(\frac{11}{5},\frac{22}{5}\right)
\end{aligned}
$$

**2. Finding the perpendicular component**

The perpendicular component is obtained by subtracting the parallel component from the original vector.

$$
\begin{aligned}
u_{\perp} &= u-u_{\parallel} \\
&= (3,4)-\left(\frac{11}{5},\frac{22}{5}\right) \\
&= \left(\frac{15}{5}-\frac{11}{5},\frac{20}{5}-\frac{22}{5}\right) \\
&= \left(\frac{4}{5},-\frac{2}{5}\right)
\end{aligned}
$$

**3. Verification of the decomposition**

The sum of the parallel and perpendicular components must equal the original vector.

$$
\begin{aligned}
u_{\parallel}+u_{\perp}
&= \left(\frac{11}{5},\frac{22}{5}\right)
+\left(\frac{4}{5},-\frac{2}{5}\right) \\
&= \left(\frac{15}{5},\frac{20}{5}\right) \\
&= (3,4) \\
&= u
\end{aligned}
$$

Therefore, the decomposition is correct.

**4. Verification of perpendicularity**

The perpendicular component must have a zero dot product with $v$.

$$
\begin{aligned}
u_{\perp}\cdot v
&= \left(\frac{4}{5},-\frac{2}{5}\right)\cdot(1,2) \\
&= \frac{4}{5}-\frac{4}{5} \\
&= 0
\end{aligned}
$$

Therefore, $u_{\perp}$ is perpendicular to $v$.

**5. Explanation of the two checks**

The first check confirms that the two components reconstruct the original vector.

The second check confirms that the perpendicular component is orthogonal to the direction of $v$.

These checks verify different properties: reconstruction alone does not prove perpendicularity, and perpendicularity alone does not prove that the original vector has been reconstructed correctly.

