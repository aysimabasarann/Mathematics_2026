### Exercise 15. Comparing Directions Using the Cosine of the Angle

#### Question
Given

$$
a=(1,2,1),\qquad b=(2,4,2),\qquad c=(2,0,3).
$$

For each pair, compute

$$
\frac{u\cdot v}{\|u\|\,\|v\|}.
$$

Order the pairs by increasing angle between the vectors. Explain why for $a$ and $b$ the value is $1$ even though the vectors have different lengths.

#### Solution
Given vectors are

$$
a = (1, 2, 1), \qquad b = (2, 4, 2), \qquad c = (2, 0, 3).
$$

**1. Lengths of the Vectors**

$$
\begin{aligned}
\|a\| &= \sqrt{1^2 + 2^2 + 1^2} \\
      &= \sqrt{1 + 4 + 1} \\
      &= \sqrt{6}
\end{aligned}
$$

$$
\begin{aligned}
\|b\| &= \sqrt{2^2 + 4^2 + 2^2} \\
      &= \sqrt{4 + 16 + 4} \\
      &= \sqrt{24} \\
      &= 2\sqrt{6}
\end{aligned}
$$

$$
\begin{aligned}
\|c\| &= \sqrt{2^2 + 0^2 + 3^2} \\
      &= \sqrt{4 + 0 + 9} \\
      &= \sqrt{13}
\end{aligned}
$$

**2. Cosine Computation for Each Pair**

* **Pair $(a, b)$:**

$$
\begin{aligned}
a \cdot b &= (1)(2) + (2)(4) + (1)(2) \\
          &= 2 + 8 + 2 \\
          &= 12
\end{aligned}
$$

$$
\begin{aligned}
\cos\theta_{ab} &= \frac{a \cdot b}{\|a\|\,\|b\|} \\
                &= \frac{12}{\sqrt{6} \cdot 2\sqrt{6}} \\
                &= \frac{12}{12} \\
                &= 1
\end{aligned}
$$

* **Pair $(a, c)$:**

$$
\begin{aligned}
a \cdot c &= (1)(2) + (2)(0) + (1)(3) \\
          &= 2 + 0 + 3 \\
          &= 5
\end{aligned}
$$

$$
\begin{aligned}
\cos\theta_{ac} &= \frac{a \cdot c}{\|a\|\,\|c\|} \\
                &= \frac{5}{\sqrt{6} \cdot \sqrt{13}} \\
                &= \frac{5}{\sqrt{78}}
\end{aligned}
$$

* **Pair $(b, c)$:**

$$
\begin{aligned}
b \cdot c &= (2)(2) + (4)(0) + (2)(3) \\
          &= 4 + 0 + 6 \\
          &= 10
\end{aligned}
$$

$$
\begin{aligned}
\cos\theta_{bc} &= \frac{b \cdot c}{\|b\|\,\|c\|} \\
                &= \frac{10}{2\sqrt{6} \cdot \sqrt{13}} \\
                &= \frac{10}{2\sqrt{78}} \\
                &= \frac{5}{\sqrt{78}}
\end{aligned}
$$

**3. Ordering the Pairs by Increasing Angle**
Because the cosine function decreases on $[0^\circ, 180^\circ]$, a larger cosine corresponds to a smaller angle. Since $1 > \frac{5}{\sqrt{78}}$, the order from smallest to largest angle is:

1. **Pair $(a, b)$:** $\theta_{ab} = \arccos(1) = 0^\circ$
2. **Pairs $(a, c)$ and $(b, c)$ (tied):** $\theta_{ac} = \theta_{bc} = \arccos\left(\frac{5}{\sqrt{78}}\right) \approx 55.5^\circ$

**4. Explanation for $a$ and $b$**
Notice that $b = (2, 4, 2) = 2(1, 2, 1) = 2a$. Because $b$ is a positive scalar multiple of $a$, both vectors point in the exact same direction and orientation, making the angle between them $0^\circ$ ($\cos 0^\circ = 1$). The expression $\frac{u \cdot v}{\|u\|\,\|v\|}$ normalizes both vectors by dividing by their lengths, so it depends solely on their directions and is completely unaffected by differences in magnitude.

 
 
