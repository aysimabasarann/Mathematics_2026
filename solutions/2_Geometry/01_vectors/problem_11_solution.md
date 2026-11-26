### Exercise 11. Decomposition into Parallel and Perpendicular Components

#### Question
Decompose $u=(3,4)$ into components parallel and perpendicular to $v=(1,2)$. Check

$$
u=u_{\parallel}+u_{\perp},\qquad u_{\perp}\cdot v=0.
$$

Explain why these are two independent checks of correctness.

#### Solution
Given vectors are

$$
u = (3, 4), \qquad v = (1, 2).
$$

**1. Parallel Component ($u_{\parallel}$)**
The parallel component is the projection of $u$ onto $v$:

$$
u_{\parallel} = \mathrm{proj}_v\,u = \frac{u \cdot v}{v \cdot v} v
$$

Computing the required dot products:

$$
\begin{aligned}
u \cdot v &= (3)(1) + (4)(2) \\
          &= 3 + 8 \\
          &= 11
\end{aligned}
$$

$$
\begin{aligned}
v \cdot v &= (1)(1) + (2)(2) \\
          &= 1 + 4 \\
          &= 5
\end{aligned}
$$

Substituting these into the formula:

$$
\begin{aligned}
u_{\parallel} &= \frac{11}{5}(1, 2) \\
              &= \left(\frac{11}{5}, \frac{22}{5}\right)
\end{aligned}
$$

**2. Perpendicular Component ($u_{\perp}$)**

$$
\begin{aligned}
u_{\perp} &= u - u_{\parallel} \\
          &= (3, 4) - \left(\frac{11}{5}, \frac{22}{5}\right) \\
          &= \left(3 - \frac{11}{5},\; 4 - \frac{22}{5}\right) \\
          &= \left(\frac{15 - 11}{5},\; \frac{20 - 22}{5}\right) \\
          &= \left(\frac{4}{5}, -\frac{2}{5}\right)
\end{aligned}
$$

**3. Verification of Checks**
* **Check 1 ($u = u_{\parallel} + u_{\perp}$):**

$$
\begin{aligned}
u_{\parallel} + u_{\perp} &= \left(\frac{11}{5}, \frac{22}{5}\right) + \left(\frac{4}{5}, -\frac{2}{5}\right) \\
                          &= \left(\frac{11 + 4}{5},\; \frac{22 - 2}{5}\right) \\
                          &= \left(\frac{15}{5},\; \frac{20}{5}\right) \\
                          &= (3, 4) \\
                          &= u \quad (\text{Verified})
\end{aligned}
$$

* **Check 2 ($u_{\perp} \cdot v = 0$):**

$$
\begin{aligned}
u_{\perp} \cdot v &= \left(\frac{4}{5}\right)(1) + \left(-\frac{2}{5}\right)(2) \\
                  &= \frac{4}{5} - \frac{4}{5} \\
                  &= 0 \quad (\text{Verified})
\end{aligned}
$$

**4. Explanation**
These are two independent checks because they test completely different mathematical properties: the first check verifies vector addition (reconstruction of the original vector), while the second check verifies orthogonality (the perpendicularity condition between the residual component and the direction vector).



