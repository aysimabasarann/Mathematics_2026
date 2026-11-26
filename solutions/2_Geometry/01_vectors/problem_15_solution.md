
### Exercise 15. Comparing Directions Using the Cosine of the Angle

Given the vectors

$$
a=(1,2,1),\quad b=(2,4,2),\quad c=(2,0,3)
$$

The cosine of the angle between two nonzero vectors is calculated using

$$
\cos\theta=\frac{u\cdot v}{\|u\|\|v\|}
$$

**1. Calculating the cosine for each pair**

First, calculate the lengths of the three vectors.

$$
\begin{aligned}
\|a\| &= \sqrt{1^2+2^2+1^2} \\
&= \sqrt{6}
\end{aligned}
$$

$$
\begin{aligned}
\|b\| &= \sqrt{2^2+4^2+2^2} \\
&= \sqrt{24}=2\sqrt{6}
\end{aligned}
$$

$$
\begin{aligned}
\|c\| &= \sqrt{2^2+0^2+3^2} \\
&= \sqrt{13}
\end{aligned}
$$

**Pair 1: Vectors $a$ and $b$**

Calculate their dot product.

$$
\begin{aligned}
a\cdot b &= 1\cdot 2+2\cdot 4+1\cdot 2 \\
&= 2+8+2 \\
&= 12
\end{aligned}
$$

Now calculate the cosine.

$$
\begin{aligned}
\cos\theta_{ab}
&= \frac{a\cdot b}{\|a\|\|b\|} \\
&= \frac{12}{\sqrt{6}\cdot 2\sqrt{6}} \\
&= \frac{12}{12} \\
&= 1
\end{aligned}
$$

**Pair 2: Vectors $a$ and $c$**

Calculate their dot product.

$$
\begin{aligned}
a\cdot c &= 1\cdot 2+2\cdot 0+1\cdot 3 \\
&= 2+0+3 \\
&= 5
\end{aligned}
$$

Now calculate the cosine.

$$
\begin{aligned}
\cos\theta_{ac}
&= \frac{a\cdot c}{\|a\|\|c\|} \\
&= \frac{5}{\sqrt{6}\sqrt{13}} \\
&= \frac{5}{\sqrt{78}}
\end{aligned}
$$

**Pair 3: Vectors $b$ and $c$**

Calculate their dot product.

$$
\begin{aligned}
b\cdot c &= 2\cdot 2+4\cdot 0+2\cdot 3 \\
&= 4+0+6 \\
&= 10
\end{aligned}
$$

Now calculate the cosine.

$$
\begin{aligned}
\cos\theta_{bc}
&= \frac{b\cdot c}{\|b\|\|c\|} \\
&= \frac{10}{2\sqrt{6}\sqrt{13}} \\
&= \frac{10}{2\sqrt{78}} \\
&= \frac{5}{\sqrt{78}}
\end{aligned}
$$

**2. Ordering the pairs by increasing angle**

The cosine function decreases as the angle increases from $0^\circ$ to $180^\circ$.

For the three pairs, the cosine values are

$$
\cos\theta_{ab}=1
$$

$$
\cos\theta_{ac}=\frac{5}{\sqrt{78}}
$$

$$
\cos\theta_{bc}=\frac{5}{\sqrt{78}}
$$

Since $1$ is greater than $\frac{5}{\sqrt{78}}$, the angle between $a$ and $b$ is smaller than the other two angles.

Therefore, the pairs are ordered by increasing angle as follows:

$$
(a,b)<(a,c)=(b,c)
$$

The corresponding angles are

$$
\theta_{ab}=0^\circ
$$

$$
\theta_{ac}=\theta_{bc}
=\cos^{-1}\left(\frac{5}{\sqrt{78}}\right)
\approx 55.5^\circ
$$

**3. Explanation of the cosine value for $a$ and $b$**

The vectors $a$ and $b$ have different lengths, but their directions are identical.

This is because

$$
b=(2,4,2)=2(1,2,1)=2a
$$

Thus, $b$ is a positive scalar multiple of $a$.

The cosine of the angle between two vectors depends on their directions, not their lengths. Since both vectors point in the same direction, the angle between them is $0^\circ$ and its cosine is equal to $1$.


