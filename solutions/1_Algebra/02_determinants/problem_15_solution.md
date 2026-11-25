
# Exercise 15 – Combining Determinant Properties

## Solution

Given:

\[
\det(A)=-2,\qquad \det(B)=3
\]

We need to compute:

\[
\det(B^{-1}A^TB)
\]

### Step 1. Apply the determinant of a product

Using the property:

\[
\det(XYZ)=\det(X)\det(Y)\det(Z)
\]

We obtain:

\[
\det(B^{-1}A^TB)
=
\det(B^{-1})\det(A^T)\det(B)
\]

### Step 2. Apply the inverse and transpose properties

We know that:

\[
\det(B^{-1})=\frac{1}{\det(B)}
\]

and

\[
\det(A^T)=\det(A)
\]

Substituting the given values:

\[
=\frac{1}{3}\cdot(-2)\cdot3
\]

### Step 3. Simplify

The factors involving \(B\) cancel:

\[
=\frac{1}{3}\cdot(-2)\cdot3
\]

\[
\boxed{-2}
\]

### Step 4. Explain why the factors cancel

The determinant of \(B^{-1}\) is the reciprocal of the determinant of \(B\).

Therefore:

\[
\det(B^{-1})\det(B)
=
\frac{1}{\det(B)}\det(B)=1
\]

This is why the factors involving \(B\) cancel.

### Final Answer

\[
\boxed{\det(B^{-1}A^TB)=-2}
\]

The properties used, in order, are:

1. Determinant of a product:
   \[
   \det(XY)=\det(X)\det(Y)
   \]

2. Determinant of an inverse:
   \[
   \det(B^{-1})=\frac{1}{\det(B)}
   \]

3. Determinant of a transpose:
   \[
   \det(A^T)=\det(A)
   \]
