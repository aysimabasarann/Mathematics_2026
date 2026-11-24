
# Problem 14 – Rotation Matrices

## Solution

The rotation matrix is:

\[
R(\theta) =
\begin{pmatrix}
\cos\theta & -\sin\theta \\
\sin\theta & \cos\theta
\end{pmatrix}
\]

### 1. Calculate R(α)R(β)

We write both matrices:

\[
R(\alpha) =
\begin{pmatrix}
\cos\alpha & -\sin\alpha \\
\sin\alpha & \cos\alpha
\end{pmatrix}
\]

\[
R(\beta) =
\begin{pmatrix}
\cos\beta & -\sin\beta \\
\sin\beta & \cos\beta
\end{pmatrix}
\]

Now multiply them:

\[
R(\alpha)R(\beta) =
\begin{pmatrix}
\cos\alpha\cos\beta-\sin\alpha\sin\beta &
-\cos\alpha\sin\beta-\sin\alpha\cos\beta \\
\sin\alpha\cos\beta+\cos\alpha\sin\beta &
-\sin\alpha\sin\beta+\cos\alpha\cos\beta
\end{pmatrix}
\]

### 2. Apply the angle-sum formulas

Using the trigonometric identities:

\[
\cos(\alpha+\beta)=
\cos\alpha\cos\beta-\sin\alpha\sin\beta
\]

\[
\sin(\alpha+\beta)=
\sin\alpha\cos\beta+\cos\alpha\sin\beta
\]

We obtain:

\[
R(\alpha)R(\beta) =
\begin{pmatrix}
\cos(\alpha+\beta) & -\sin(\alpha+\beta) \\
\sin(\alpha+\beta) & \cos(\alpha+\beta)
\end{pmatrix}
\]

Therefore,

\[
\boxed{R(\alpha)R(\beta)=R(\alpha+\beta)}
\]

### 3. Geometrical explanation

A rotation by an angle β followed by a rotation by an angle α is equivalent to a single rotation by the sum of these angles.

Both rotations are performed around the same origin and in the same direction.

Therefore, the total rotation angle is α + β.

### Final Answer

\[
\boxed{R(\alpha)R(\beta)=R(\alpha+\beta)}
\]

The composition of two rotations is another rotation whose angle is the sum of the original angles.
