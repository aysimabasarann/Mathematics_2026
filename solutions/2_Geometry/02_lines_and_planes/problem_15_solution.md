### Exercise 15. Complete Classification of a Line Relative to a Plane

#### Question
Let

$$
L:p+tv,\qquad \Pi:n\cdot x=d.
$$

State the conditions distinguishing the three cases: one intersection point, parallel with no common points, and the line contained in the plane. Then illustrate each case with your own simple numerical example.

#### Solution
Substituting the general point of the line $x = p + tv$ into the plane equation $n \cdot x = d$ yields

$$
\begin{aligned}
n \cdot (p + tv) &= d \\
n \cdot p + t(n \cdot v) &= d \\
(n \cdot v)t &= d - n \cdot p
\end{aligned}
$$

**1. Conditions Distinguishing the Three Cases**

* **Case 1: One intersection point**
  * **Condition:** $n \cdot v \neq 0$.
  * **Reason:** The direction vector $v$ is not perpendicular to the normal vector $n$, so the equation $(n \cdot v)t = d - n \cdot p$ has a unique solution $t = \frac{d - n \cdot p}{n \cdot v}$.

* **Case 2: Parallel with no common points (strictly parallel)**
  * **Condition:** $n \cdot v = 0$ and $n \cdot p \neq d$.
  * **Reason:** The line runs parallel to the plane ($n \cdot v = 0$), and its starting point $p$ does not lie on the plane ($d - n \cdot p \neq 0$), leading to $0 \cdot t = d - n \cdot p \neq 0$ (no solution).

* **Case 3: The line is contained in the plane**
  * **Condition:** $n \cdot v = 0$ and $n \cdot p = d$.
  * **Reason:** The line is parallel to the plane ($n \cdot v = 0$) and at least one point $p$ lies in the plane ($d - n \cdot p = 0$), leading to $0 \cdot t = 0$ (satisfied for all $t \in \mathbb{R}$).

---

**2. Simple Numerical Examples**
Let the plane $\Pi$ be $z = 1$, which has normal vector $n = (0, 0, 1)$ and constant $d = 1$.

* **Example for Case 1 (One intersection point):**
  Let $L_1: (0, 0, 0) + t(0, 0, 1)$, so $p = (0, 0, 0)$ and $v = (0, 0, 1)$.
  * Check: $n \cdot v = (0, 0, 1) \cdot (0, 0, 1) = 1 \neq 0$.
  * Intersection: Setting $z = t = 1$ gives the unique intersection point $(0, 0, 1)$.

* **Example for Case 2 (Parallel with no common points):**
  Let $L_2: (0, 0, 2) + t(1, 0, 0)$, so $p = (0, 0, 2)$ and $v = (1, 0, 0)$.
  * Check: $n \cdot v = (0, 0, 1) \cdot (1, 0, 0) = 0$, while $n \cdot p = (0, 0, 1) \cdot (0, 0, 2) = 2 \neq 1$.
  * Result: Every point on $L_2$ has $z = 2$, so it never meets the plane $z = 1$.

* **Example for Case 3 (Line contained in the plane):**
  Let $L_3: (0, 0, 1) + t(1, 0, 0)$, so $p = (0, 0, 1)$ and $v = (1, 0, 0)$.
  * Check: $n \cdot v = (0, 0, 1) \cdot (1, 0, 0) = 0$, and $n \cdot p = (0, 0, 1) \cdot (0, 0, 1) = 1 = d$.
  * Result: Every point $(t, 0, 1)$ on $L_3$ satisfies $z = 1$, so the entire line lies inside the plane.
