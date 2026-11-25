### Exercise 11. When Do Matrices Commute?

**Problem:**

Given

$$
A = \begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix},\qquad B = \begin{pmatrix}
a & b \\
c & d
\end{pmatrix}.
$$

Find the conditions on $a, b, c, d$ under which $AB = BA$. Describe the general form of all such matrices $B$.

---

## Solution

### 1. Computing the Product $AB$

First, we multiply $A$ on the left by $B$ on the right:

$$
AB = \begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
a & b \\
c & d
\end{pmatrix}
= \begin{pmatrix}
(1)(a) + (1)(c) & (1)(b) + (1)(d) \\
(0)(a) + (1)(c) & (0)(b) + (1)(d)
\end{pmatrix}
= \begin{pmatrix}
a + c & b + d \\
c & d
\end{pmatrix}
$$

### 2. Computing the Product $BA$

Next, we multiply $B$ on the left by $A$ on the right:

$$
BA = \begin{pmatrix}
a & b \\
c & d
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
= \begin{pmatrix}
(a)(1) + (b)(0) & (a)(1) + (b)(1) \\
(c)(1) + (d)(0) & (c)(1) + (d)(1)
\end{pmatrix}
= \begin{pmatrix}
a & a + b \\
c & c + d
\end{pmatrix}
$$

### 3. Equating $AB$ and $BA$ to Find Conditions

For $AB = BA$ to hold, every corresponding entry of the two resulting matrices must be equal:

$$
\begin{pmatrix}
a + c & b + d \\
c & d
\end{pmatrix}
=
\begin{pmatrix}
a & a + b \\
c & c + d
\end{pmatrix}
$$

Comparing the entries one by one gives the following system of equations:

1. Top-left entry: $a + c = a \implies c = 0$
2. Top-right entry: $b + d = a + b \implies d = a$
3. Bottom-left entry: $c = c$ (always satisfied)
4. Bottom-right entry: $d = c + d \implies c = 0$

Thus, the necessary and sufficient conditions for $AB = BA$ are:

$$
c = 0, \qquad a = d
$$

### 4. General Form and Verification

Substituting $c = 0$ and $d = a$ into $B$, every matrix $B$ that commutes with $A$ has the general upper-triangular form:

$$
B = \begin{pmatrix}
a & b \\
0 & a
\end{pmatrix}
$$

where $a$ and $b$ are arbitrary real numbers.

**Verification:**
Checking the products with this general form confirms commutativity:

$$
AB = \begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
a & b \\
0 & a
\end{pmatrix}
= \begin{pmatrix}
a & a + b \\
0 & a
\end{pmatrix}
$$

$$
BA = \begin{pmatrix}
a & b \\
0 & a
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
= \begin{pmatrix}
a & a + b \\
0 & a
\end{pmatrix}
$$

Since $AB = BA$ holds for all $a, b \in \mathbb{R}$, the result is verified.

