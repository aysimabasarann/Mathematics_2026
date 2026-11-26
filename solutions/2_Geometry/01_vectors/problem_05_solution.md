### Exercise 5. Angle Between Vectors

#### Question
Given $u=(1,1,0)$ and $v=(1,0,1)$:

1. Use the sign of $u\cdot v$ to predict the type of angle.
2. Compute the angle.
3. Compare the result with the prediction.

#### Solution
Given vectors are

$$
u = (1, 1, 0), \qquad v = (1, 0, 1).
$$

**1. Prediction Using the Sign of $u \cdot v$**

$$
\begin{aligned}
u \cdot v &= (1)(1) + (1)(0) + (0)(1) \\
          &= 1 + 0 + 0 \\
          &= 1
\end{aligned}
$$

Since $u \cdot v = 1 > 0$, the dot product is positive. Therefore, the angle $\theta$ between $u$ and $v$ is predicted to be an acute angle ($0^\circ \le \theta < 90^\circ$).

**2. Computation of the Angle**
First, compute the lengths of both vectors:

$$
\begin{aligned}
\|u\| &= \sqrt{1^2 + 1^2 + 0^2} \\
      &= \sqrt{2}
\end{aligned}
$$

$$
\begin{aligned}
\|v\| &= \sqrt{1^2 + 0^2 + 1^2} \\
      &= \sqrt{2}
\end{aligned}
$$

Using the geometric definition of the dot product, $\cos\theta = \frac{u \cdot v}{\|u\|\,\|v\|}$:

$$
\begin{aligned}
\cos\theta &= \frac{1}{\sqrt{2} \cdot \sqrt{2}} \\
           &= \frac{1}{2}
\end{aligned}
$$

Taking the inverse cosine gives

$$
\theta = \arccos\left(\frac{1}{2}\right) = 60^\circ = \frac{\pi}{3}.
$$

**3. Comparison with the Prediction**
The computed angle is $60^\circ$ (or $\frac{\pi}{3}$ radians), which satisfies $0^\circ \le 60^\circ < 90^\circ$. This confirms our initial prediction that the angle between the vectors is acute.



