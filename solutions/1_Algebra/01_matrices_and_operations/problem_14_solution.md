### Exercise 14. Rotation Matrices

**Problem:**

The matrix for a rotation through an angle $\theta$ is

$$
R(\theta) = \begin{pmatrix} \cos\theta & -\sin\theta \\ \sin\theta & \cos\theta \end{pmatrix}.
$$

Compute $R(\alpha)R(\beta)$ and, using the angle-sum formulas for sine and cosine, show that

$$
R(\alpha)R(\beta) = R(\alpha+\beta).
$$

Explain the result geometrically.

---

## Solution

### 1. Computing the Product $R(\alpha)R(\beta)$

We multiply the two rotation matrices corresponding to angles $\alpha$ and $\beta$:

$$
R(\alpha)R(\beta) = \begin{pmatrix} \cos\alpha & -\sin\alpha \\ \sin\alpha & \cos\alpha \end{pmatrix} \begin{pmatrix} \cos\beta & -\sin\beta \\ \sin\beta & \cos\beta \end{pmatrix}
$$

Carrying out matrix multiplication:

$$
R(\alpha)R(\beta) = \begin{pmatrix} (\cos\alpha)(\cos\beta) + (-\sin\alpha)(\sin\beta) & (\cos\alpha)(-\sin\beta) + (-\sin\alpha)(\cos\beta) \\ (\sin\alpha)(\cos\beta) + (\cos\alpha)(\sin\beta) & (\sin\alpha)(-\sin\beta) + (\cos\alpha)(\cos\beta) \end{pmatrix}
$$

Rewriting the entries neatly:

$$
R(\alpha)R(\beta) = \begin{pmatrix} \cos\alpha\cos\beta - \sin\alpha\sin\beta & -(\sin\alpha\cos\beta + \cos\alpha\sin\beta) \\ \sin\alpha\cos\beta + \cos\alpha\sin\beta & \cos\alpha\cos\beta - \sin\alpha\sin\beta \end{pmatrix}
$$

### 2. Applying Trigonometric Angle-Sum Formulas

Using the standard angle-sum trigonometric identities:
* $\cos(\alpha + \beta) = \cos\alpha\cos\beta - \sin\alpha\sin\beta$
* $\sin(\alpha + \beta) = \sin\alpha\cos\beta + \cos\alpha\sin\beta$

Substituting these identities into each entry of our product matrix:

$$
R(\alpha)R(\beta) = \begin{pmatrix} \cos(\alpha + \beta) & -\sin(\alpha + \beta) \\ \sin(\alpha + \beta) & \cos(\alpha + \beta) \end{pmatrix}
$$

By definition of the rotation matrix, this final matrix is precisely $R(\alpha + \beta)$:

$$
R(\alpha)R(\beta) = R(\alpha + \beta)
$$

### 3. Geometric Explanation

**Geometric Interpretation:**
Matrix multiplication of rotation matrices represents the composition of linear geometric transformations. 
* Multiplying by $R(\beta)$ first rotates a vector by an angle $\beta$ around the origin.
* Subsequent multiplication by $R(\alpha)$ rotates that resulting vector by an additional angle $\alpha$.

Rotating a vector first by $\beta$ and then by $\alpha$ in the counterclockwise direction is geometrically equivalent to performing a single rotation by the combined angle $\alpha + \beta$. Thus, matrix multiplication accurately reflects the composition of rotational geometry.

