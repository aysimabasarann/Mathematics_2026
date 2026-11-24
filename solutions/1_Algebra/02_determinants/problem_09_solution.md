
# Problem 09 – Area and the Determinant

## Solution

Given:

\[
u=\begin{pmatrix}3\\1\end{pmatrix},
\qquad
v=\begin{pmatrix}1\\4\end{pmatrix}
\]

### 1. Calculate the determinant

Place the vectors as columns of a matrix:

\[
A=\begin{pmatrix}
3 & 1\\
1 & 4
\end{pmatrix}
\]

For a 2x2 matrix, the determinant is:

\[
\det(A)=ad-bc
\]

Substituting the values:

\[
\det(A)=3\cdot4-1\cdot1
\]

\[
\det(A)=12-1
\]

\[
\boxed{\det(A)=11}
\]

### 2. Calculate the area of the parallelogram

The area of a parallelogram formed by two vectors is the absolute value of the determinant.

Therefore:

\[
\text{Area}=|\det(A)|
\]

\[
\text{Area}=|11|
\]

\[
\boxed{\text{Area}=11}
\]

### 3. Reverse the order of the vectors

Now place the vectors in the opposite order:

\[
B=\begin{pmatrix}
1 & 3\\
4 & 1
\end{pmatrix}
\]

Calculate the new determinant:

\[
\det(B)=1\cdot1-3\cdot4
\]

\[
\det(B)=1-12
\]

\[
\boxed{\det(B)=-11}
\]

### 4. Compare the results

When two columns of a matrix are swapped, the determinant changes its sign.

Therefore:

\[
\det(B)=-\det(A)
\]

However, the area is the absolute value of the determinant.

\[
\text{Area}=|-11|=11
\]

Thus, the area does not change.

### Final Answer

Original determinant:

\[
\boxed{\det(A)=11}
\]

Reversed determinant:

\[
\boxed{\det(B)=-11}
\]

Area of the parallelogram:

\[
\boxed{\text{Area}=11}
\]

Reversing the order of the vectors changes the sign of the determinant, but the area remains the same because area is always nonnegative.
