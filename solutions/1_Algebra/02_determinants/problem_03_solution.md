
# Problem 03 – Swapping Two Rows

## Solution

Given:

\[
A = \begin{pmatrix}
1 & 2 & 0 \\
0 & 3 & 1 \\
2 & 1 & 1
\end{pmatrix}
\]

### 1. Calculate the determinant of A

Using the determinant formula for a 3x3 matrix:

\[
\det(A)=
1(3\cdot1-1\cdot1)
-2(0\cdot1-1\cdot2)
+0
\]

Simplifying:

\[
\det(A)=1(3-1)-2(0-2)
\]

\[
\det(A)=2+4
\]

\[
\boxed{\det(A)=6}
\]

### 2. Form matrix B by swapping the first and second rows

After swapping the first and second rows, we obtain:

\[
B = \begin{pmatrix}
0 & 3 & 1 \\
1 & 2 & 0 \\
2 & 1 & 1
\end{pmatrix}
\]

### 3. Predict the determinant of B

One important property of determinants states that swapping two rows changes the sign of the determinant.

Therefore:

\[
\det(B)=-\det(A)
\]

Since:

\[
\det(A)=6
\]

We predict:

\[
\boxed{\det(B)=-6}
\]

### 4. Verify the result by calculation

Calculating the determinant of B:

\[
\det(B)=
0(2\cdot1-0\cdot1)
-3(1\cdot1-0\cdot2)
+1(1\cdot1-2\cdot2)
\]

Simplifying:

\[
\det(B)=0-3(1)+(1-4)
\]

\[
\det(B)=-3-3
\]

\[
\boxed{\det(B)=-6}
\]

The calculated result agrees with our prediction.

### Final Answer

\[
\boxed{\det(A)=6}
\]

\[
\boxed{\det(B)=-6}
\]

Swapping two rows of a matrix changes the sign of its determinant but does not change its absolute value.
