### Exercise 3. Vector Normalization

#### Question
For $v=(3,4)$ find a unit vector $e$ with the same direction and orientation. Check that $\|e\|=1$, reconstruct $v$ in the form $v=\|v\|e$, and explain what changes during normalization and what remains unchanged.

#### Solution
Given vector is

$$
v = (3, 4).
$$

**1. Length of $v$**

$$
\begin{aligned}
\|v\| &= \sqrt{3^2 + 4^2} \\
      &= \sqrt{9 + 16} \\
      &= \sqrt{25} \\
      &= 5
\end{aligned}
$$

**2. Unit Vector $e$**

$$
\begin{aligned}
e &= \frac{v}{\|v\|} \\
  &= \frac{1}{5}(3, 4) \\
  &= \left(\frac{3}{5}, \frac{4}{5}\right)
\end{aligned}
$$

**3. Verification of $\|e\| = 1$**

$$
\begin{aligned}
\|e\| &= \sqrt{\left(\frac{3}{5}\right)^2 + \left(\frac{4}{5}\right)^2} \\
      &= \sqrt{\frac{9}{25} + \frac{16}{25}} \\
      &= \sqrt{\frac{25}{25}} \\
      &= 1
\end{aligned}
$$

**4. Reconstruction of $v$**

$$
\begin{aligned}
\|v\|e &= 5\left(\frac{3}{5}, \frac{4}{5}\right) \\
       &= (3, 4) \\
       &= v
\end{aligned}
$$

**5. Explanation**
During normalization, the length (magnitude) of the vector is scaled to $1$. However, both the direction and the orientation of the vector remain completely unchanged.




