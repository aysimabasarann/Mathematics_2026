
# Exercise 14 – A System of Equations and the Determinant

## Solution

Given:

\[
A=
\begin{pmatrix}
1&2\\
k&4
\end{pmatrix}
\]

### Step 1. Calculate the determinant

\[
\det(A)=1\cdot4-2\cdot k
\]

\[
\det(A)=4-2k
\]

### Step 2. Find the condition for a unique solution

A system has exactly one solution for every \(b\) if and only if its coefficient matrix is invertible.

Therefore:

\[
\det(A)\neq0
\]

\[
4-2k\neq0
\]

\[
2k\neq4
\]

\[
\boxed{k\neq2}
\]

### Step 3. Consider the remaining value

When \(k=2\), the matrix becomes:

\[
A=
\begin{pmatrix}
1&2\\
2&4
\end{pmatrix}
\]

The system is:

\[
\begin{cases}
x_1+2x_2=b_1\\
2x_1+4x_2=b_2
\end{cases}
\]

The second equation is twice the first equation.

### Step 4. Example with infinitely many solutions

Choose:

\[
b=
\begin{pmatrix}
1\\
2
\end{pmatrix}
\]

The system becomes:

\[
\begin{cases}
x_1+2x_2=1\\
2x_1+4x_2=2
\end{cases}
\]

Both equations represent the same line.

Therefore, there are infinitely many solutions.

### Step 5. Example with no solution

Choose:

\[
b=
\begin{pmatrix}
1\\
0
\end{pmatrix}
\]

The system becomes:

\[
\begin{cases}
x_1+2x_2=1\\
2x_1+4x_2=0
\end{cases}
\]

The second equation contradicts the first equation.

Therefore, there is no solution.

### Final Answer

- Exactly one solution for every \(b\): 

\[
\boxed{k\neq2}
\]

- Infinitely many solutions when \(k=2\) and:

\[
b=\begin{pmatrix}1\\2\end{pmatrix}
\]

- No solution when \(k=2\) and:

\[
b=\begin{pmatrix}1\\0\end{pmatrix}
\]

The determinant determines whether the matrix is invertible and therefore whether the system has a unique solution for every right-hand side.
