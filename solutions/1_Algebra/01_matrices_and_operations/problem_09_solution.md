### Exercise 9. Composing Transformations

**Problem:**

Let

$$
S = \begin{pmatrix}
2 & 0 \\
0 & 1
\end{pmatrix},\qquad R = \begin{pmatrix}
0 & -1 \\
1 & 0
\end{pmatrix}
$$

The matrix $S$ describes nonuniform scaling, while $R$ describes a $90^\circ$ counterclockwise rotation.
For

$$
x = \begin{pmatrix}
1 \\
2
\end{pmatrix}
$$

compute $RSx$ and $SRx$. Compare the results and explain geometrically why the order of these transformations matters.

---

## Solution

### 1. Computing $RSx$

First, we compute the scaling of vector $x$ by evaluating $Sx$:

$$
Sx = \begin{pmatrix}
2 & 0 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
1 \\
2
\end{pmatrix}
= \begin{pmatrix}
(2)(1) + (0)(2) \\
(0)(1) + (1)(2)
\end{pmatrix}
= \begin{pmatrix}
2 \\
2
\end{pmatrix}
$$

Next, we apply the rotation matrix $R$ to the resulting vector ($RSx$):

$$
RSx = \begin{pmatrix}
0 & -1 \\
1 & 0
\end{pmatrix}
\begin{pmatrix}
2 \\
2
\end{pmatrix}
= \begin{pmatrix}
(0)(2) + (-1)(2) \\
(1)(2) + (0)(2)
\end{pmatrix}
= \begin{pmatrix}
-2 \\
2
\end{pmatrix}
$$

### 2. Computing $SRx$

First, we compute the rotation of vector $x$ by evaluating $Rx$:

$$
Rx = \begin{pmatrix}
0 & -1 \\
1 & 0
\end{pmatrix}
\begin{pmatrix}
1 \\
2
\end{pmatrix}
= \begin{pmatrix}
(0)(1) + (-1)(2) \\
(1)(1) + (0)(2)
\end{pmatrix}
= \begin{pmatrix}
-2 \\
1
\end{pmatrix}
$$

Next, we apply the scaling matrix $S$ to the resulting vector ($SRx$):

$$
SRx = \begin{pmatrix}
2 & 0 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
-2 \\
1
\end{pmatrix}
= \begin{pmatrix}
(2)(-2) + (0)(1) \\
(0)(-2) + (1)(1)
\end{pmatrix}
= \begin{pmatrix}
-4 \\
1
\end{pmatrix}
$$

### 3. Comparison and Geometric Explanation

Comparing the results:

$$
RSx = \begin{pmatrix}
-2 \\
2
\end{pmatrix}
\neq
\begin{pmatrix}
-4 \\
1
\end{pmatrix}
= SRx
$$

**Geometric Explanation:**
The order of transformations matters because matrix multiplication corresponds to the composition of linear transformations. 
* In $RSx$, vector $x$ is first stretched horizontally by a factor of $2$ (scaling $S$) and then rotated counterclockwise by $90^\circ$ ($R$).
* In $SRx$, vector $x$ is first rotated counterclockwise by $90^\circ$ ($R$) and then stretched horizontally by a factor of $2$ relative to the original coordinate axes ($S$). 

Because geometric transformations are generally not commutative, performing them in a different sequence alters the final position of the vector.

 

 
