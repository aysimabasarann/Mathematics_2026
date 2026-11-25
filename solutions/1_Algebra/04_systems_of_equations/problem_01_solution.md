 ### Exercise 1. From a System to a Matrix

Write the system

$$
\begin{cases}
2x-y+z=4, \\
x+3y-2z=1, \\
3x+y+z=7.
\end{cases}
$$

in the form $Ax=b$.
Identify the coefficient matrix, the vector of unknowns, and the right-hand side vector. Explain how each row of the matrix corresponds to one equation.

---

## Solution

### 1. Matrix Representation

The given system of linear equations can be written in the matrix form $Ax = b$ as

$$
\begin{pmatrix}
2 & -1 & 1 \\
1 & 3 & -2 \\
3 & 1 & 1 \\
\end{pmatrix}
\begin{pmatrix}
x \\
y \\
z \\
\end{pmatrix} =
\begin{pmatrix}
4 \\
1 \\
7 \\
\end{pmatrix}
$$

### 2. Identification of Components

The coefficient matrix $A$ is

$$
A =
\begin{pmatrix}
2 & -1 & 1 \\
1 & 3 & -2 \\
3 & 1 & 1 \\
\end{pmatrix}
$$

The vector of unknowns $x$ is

$$
x =
\begin{pmatrix}
x \\
y \\
z \\
\end{pmatrix}
$$

The right-hand side vector $b$ is

$$
b =
\begin{pmatrix}
4 \\
1 \\
7 \\
\end{pmatrix}
$$

### 3. Correspondence Between Rows and Equations

Each row of the matrix equation $Ax = b$ represents one scalar linear equation from the original system. Multiplying the $i$-th row of the coefficient matrix $A$ by the column vector of unknowns $x$ gives the left-hand side of the $i$-th equation, which equals the $i$-th entry of the right-hand side vector $b$:

- **Row 1:** multiplying the first row $(2, -1, 1)$ by the vector of unknowns yields $2x - y + z = 4$, which is the first equation.
- **Row 2:** multiplying the second row $(1, 3, -2)$ by the vector of unknowns yields $x + 3y - 2z = 1$, which is the second equation.
- **Row 3:** multiplying the third row $(3, 1, 1)$ by the vector of unknowns yields $3x + y + z = 7$, which is the third equation.

