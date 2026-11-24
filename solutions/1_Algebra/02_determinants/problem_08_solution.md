
# Problem 08 – Determinant of a Product

## Solution

Given:

\[
\det(A)=3,\qquad \det(B)=-5
\]

### 1. Calculate det(AB)

Using the determinant property:

\[
\det(AB)=\det(A)\cdot\det(B)
\]

Substituting the given values:

\[
\det(AB)=3\cdot(-5)
\]

\[
\boxed{\det(AB)=-15}
\]

### 2. Calculate det(BA)

Using the same property:

\[
\det(BA)=\det(B)\cdot\det(A)
\]

Substituting:

\[
\det(BA)=(-5)\cdot3
\]

\[
\boxed{\det(BA)=-15}
\]

Therefore:

\[
\det(AB)=\det(BA)
\]

### 3. Calculate det(A^{-1}B)

First, since:

\[
\det(A)=3\neq0
\]

the matrix A is invertible, so its inverse exists.

We use the property:

\[
\det(A^{-1})=\frac{1}{\det(A)}
\]

Therefore:

\[
\det(A^{-1})=\frac{1}{3}
\]

Now:

\[
\det(A^{-1}B)=\det(A^{-1})\cdot\det(B)
\]

Substituting:

\[
\det(A^{-1}B)=\frac{1}{3}\cdot(-5)
\]

\[
\boxed{\det(A^{-1}B)=-\frac{5}{3}}
\]

### 4. Explanation

Matrix multiplication is generally not commutative, which means:

\[
AB\neq BA
\]

However, their determinants are equal because:

\[
\det(AB)=\det(A)\det(B)
\]

and

\[
\det(BA)=\det(B)\det(A)
\]

Since multiplication of real numbers is commutative:

\[
\det(A)\det(B)=\det(B)\det(A)
\]

Therefore:

\[
\det(AB)=\det(BA)
\]

even when the matrices AB and BA are different.

### Final Answer

\[
\boxed{\det(AB)=-15}
\]

\[
\boxed{\det(BA)=-15}
\]

\[
\boxed{\det(A^{-1}B)=-\frac{5}{3}}
\]

The first two determinants are equal because the determinant of a matrix product is the product of the individual determinants.
