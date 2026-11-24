
# Problem 11 – When Do Matrices Commute?

## Solution

Given:

\[
A = \begin{pmatrix} 1 & 1 \\ 0 & 1 \end{pmatrix},
\quad
B = \begin{pmatrix} a & b \\ c & d \end{pmatrix}
\]

### 1. Calculate AB

\[
AB =
\begin{pmatrix} 1 & 1 \\ 0 & 1 \end{pmatrix}
\begin{pmatrix} a & b \\ c & d \end{pmatrix}
\]

\[
AB =
\begin{pmatrix}
a+c & b+d \\
c & d
\end{pmatrix}
\]

### 2. Calculate BA

\[
BA =
\begin{pmatrix} a & b \\ c & d \end{pmatrix}
\begin{pmatrix} 1 & 1 \\ 0 & 1 \end{pmatrix}
\]

\[
BA =
\begin{pmatrix}
a & a+b \\
c & c+d
\end{pmatrix}
\]

### 3. Find the conditions for AB = BA

For the matrices to be equal, their corresponding entries must be equal.

\[
a+c=a
\]

\[
b+d=a+b
\]

\[
c=c
\]

\[
d=c+d
\]

Simplifying these equations:

\[
c=0
\]

\[
d=a
\]

The third equation is automatically satisfied.

Therefore, the conditions are:

\[
c=0,\quad d=a
\]

### 4. General form of matrix B

Substituting these conditions into B:

\[
B = \begin{pmatrix} a & b \\ 0 & a \end{pmatrix}
\]

Here, a and b can be any real numbers.

### Final Answer

The matrices commute when:

\[
\boxed{c=0,\quad d=a}
\]

The general form of all such matrices is:

\[
\boxed{
B = \begin{pmatrix} a & b \\ 0 & a \end{pmatrix}
}
\]

Thus, AB = BA only when B has this form.
