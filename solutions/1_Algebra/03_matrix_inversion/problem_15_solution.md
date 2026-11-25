
# Exercise 15 – Two Methods for Solving the Same System

## Given

\[
A=
\begin{pmatrix}
2&1\\
1&3
\end{pmatrix},
\qquad
b=
\begin{pmatrix}
7\\
8
\end{pmatrix}
\]

We need to solve:

\[
Ax=b
\]

using two different methods.

## Method 1: Using the Inverse Matrix

The formula is:

\[
x=A^{-1}b
\]

### Step 1: Calculate the determinant

\[
\det(A)=2(3)-1(1)
\]

\[
\det(A)=6-1=5
\]

Since the determinant is not zero, the inverse exists.

### Step 2: Find the inverse

For a 2 × 2 matrix:

\[
A^{-1}=\frac{1}{ad-bc}
\begin{pmatrix}
d&-b\\
-c&a
\end{pmatrix}
\]

Therefore:

\[
A^{-1}=\frac{1}{5}
\begin{pmatrix}
3&-1\\
-1&2
\end{pmatrix}
\]

### Step 3: Calculate x

\[
x=A^{-1}b
\]

\[
x=\frac{1}{5}
\begin{pmatrix}
3&-1\\
-1&2
\end{pmatrix}
\begin{pmatrix}
7\\
8
\end{pmatrix}
\]

Multiplying:

\[
x=\frac{1}{5}
\begin{pmatrix}
21-8\\
-7+16
\end{pmatrix}
\]

\[
\boxed{
x=
\begin{pmatrix}
13/5\\
9/5
\end{pmatrix}
}
\]

## Method 2: Using Gaussian Elimination

Start with the augmented matrix:

\[
\left[
\begin{array}{cc|c}
2&1&7\\
1&3&8
\end{array}
\right]
\]

### Step 1: Swap the rows

\[
R_1\leftrightarrow R_2
\]

\[
\left[
\begin{array}{cc|c}
1&3&8\\
2&1&7
\end{array}
\right]
\]

### Step 2: Eliminate the first entry in the second row

\[
R_2\leftarrow R_2-2R_1
\]

\[
\left[
\begin{array}{cc|c}
1&3&8\\
0&-5&-9
\end{array}
\right]
\]

### Step 3: Make the second pivot equal to 1

\[
R_2\leftarrow-\frac{1}{5}R_2
\]

\[
\left[
\begin{array}{cc|c}
1&3&8\\
0&1&9/5
\end{array}
\right]
\]

### Step 4: Eliminate the second entry in the first row

\[
R_1\leftarrow R_1-3R_2
\]

\[
\left[
\begin{array}{cc|c}
1&0&13/5\\
0&1&9/5
\end{array}
\right]
\]

Therefore:

\[
\boxed{
x=
\begin{pmatrix}
13/5\\
9/5
\end{pmatrix}
}
\]

## Comparison of Both Methods

Both methods give the same solution.

\[
x=
\begin{pmatrix}
13/5\\
9/5
\end{pmatrix}
\]

**Method 1: Inverse Matrix**
- Calculate the determinant.
- Find the inverse matrix.
- Multiply the inverse by b.
- Requires three main calculation stages.

**Method 2: Gaussian Elimination**
- Construct the augmented matrix.
- Perform row operations.
- Obtain the solution directly.
- Requires four row operations in this example.

## Conclusion

Both methods produce the same answer.

In this example, the inverse matrix method is simpler because the matrix is only 2 × 2 and its inverse is easy to calculate.

Gaussian elimination is also effective, especially for larger systems where calculating the inverse matrix may be more complicated.
