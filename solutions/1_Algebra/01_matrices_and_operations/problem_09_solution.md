
# Problem 09 – Composing Transformations

## Solution

Given:

\[
S = \begin{pmatrix} 2 & 0 \\ 0 & 1 \end{pmatrix},
\quad
R = \begin{pmatrix} 0 & -1 \\ 1 & 0 \end{pmatrix}
\]

\[
x = \begin{pmatrix} 1 \\ 2 \end{pmatrix}
\]

### 1. Calculate RSx

First, we calculate Sx.

\[
Sx =
\begin{pmatrix} 2 & 0 \\ 0 & 1 \end{pmatrix}
\begin{pmatrix} 1 \\ 2 \end{pmatrix}
\]

\[
Sx = \begin{pmatrix} 2 \\ 2 \end{pmatrix}
\]

Now, multiply the result by R.

\[
RSx =
\begin{pmatrix} 0 & -1 \\ 1 & 0 \end{pmatrix}
\begin{pmatrix} 2 \\ 2 \end{pmatrix}
\]

\[
RSx =
\begin{pmatrix} -2 \\ 2 \end{pmatrix}
\]

### 2. Calculate SRx

First, we calculate Rx.

\[
Rx =
\begin{pmatrix} 0 & -1 \\ 1 & 0 \end{pmatrix}
\begin{pmatrix} 1 \\ 2 \end{pmatrix}
\]

\[
Rx = \begin{pmatrix} -2 \\ 1 \end{pmatrix}
\]

Now, multiply the result by S.

\[
SRx =
\begin{pmatrix} 2 & 0 \\ 0 & 1 \end{pmatrix}
\begin{pmatrix} -2 \\ 1 \end{pmatrix}
\]

\[
SRx =
\begin{pmatrix} -4 \\ 1 \end{pmatrix}
\]

### 3. Compare the results

\[
RSx = \begin{pmatrix} -2 \\ 2 \end{pmatrix}
\]

\[
SRx = \begin{pmatrix} -4 \\ 1 \end{pmatrix}
\]

Therefore,

\[
RSx \neq SRx
\]

### 4. Geometrical explanation

The matrix S doubles the x-coordinate while keeping the y-coordinate unchanged.

The matrix R rotates a vector 90 degrees counterclockwise.

When we apply S first and then R, we get:

\[
RSx = \begin{pmatrix} -2 \\ 2 \end{pmatrix}
\]

When we apply R first and then S, we get:

\[
SRx = \begin{pmatrix} -4 \\ 1 \end{pmatrix}
\]

The results are different because the order of transformations changes the final position of the vector.

### Final Answer

\[
\boxed{RSx = \begin{pmatrix} -2 \\ 2 \end{pmatrix}}
\]

\[
\boxed{SRx = \begin{pmatrix} -4 \\ 1 \end{pmatrix}}
\]

Matrix transformations are not generally commutative because changing their order can produce different results.
