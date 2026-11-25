
# Exercise 7 – Inverse of a Product

## Solution

Given:

\[
A=
\begin{pmatrix}
1&1\\
0&1
\end{pmatrix},
\qquad
B=
\begin{pmatrix}
2&0\\
0&3
\end{pmatrix}
\]

### Step 1. Calculate AB

\[
AB=
\begin{pmatrix}
1&1\\
0&1
\end{pmatrix}
\begin{pmatrix}
2&0\\
0&3
\end{pmatrix}
\]

\[
AB=
\begin{pmatrix}
2&3\\
0&3
\end{pmatrix}
\]

### Step 2. Find (AB)⁻¹

Using the inverse formula:

\[
(AB)^{-1}
=
\frac{1}{6}
\begin{pmatrix}
3&-3\\
0&2
\end{pmatrix}
\]

Therefore:

\[
(AB)^{-1}
=
\begin{pmatrix}
\frac12&-\frac12\\
0&\frac13
\end{pmatrix}
\]

### Step 3. Calculate A⁻¹ and B⁻¹

First:

\[
A^{-1}=
\begin{pmatrix}
1&-1\\
0&1
\end{pmatrix}
\]

And:

\[
B^{-1}=
\begin{pmatrix}
\frac12&0\\
0&\frac13
\end{pmatrix}
\]

### Step 4. Calculate B⁻¹A⁻¹

\[
B^{-1}A^{-1}
=
\begin{pmatrix}
\frac12&0\\
0&\frac13
\end{pmatrix}
\begin{pmatrix}
1&-1\\
0&1
\end{pmatrix}
\]

\[
=
\begin{pmatrix}
\frac12&-\frac12\\
0&\frac13
\end{pmatrix}
\]

### Step 5. Compare the Results

We obtain:

\[
(AB)^{-1}
=
\begin{pmatrix}
\frac12&-\frac12\\
0&\frac13
\end{pmatrix}
\]

and

\[
B^{-1}A^{-1}
=
\begin{pmatrix}
\frac12&-\frac12\\
0&\frac13
\end{pmatrix}
\]

Therefore:

\[
\boxed{(AB)^{-1}=B^{-1}A^{-1}}
\]

### Explanation of the Reversed Order

The inverse of a product reverses the order of multiplication.

When applying AB to a vector, B acts first and then A. To undo these operations, we must first undo A and then undo B.

This is why:

\[
\boxed{(AB)^{-1}=B^{-1}A^{-1}}
\]

The results are equal, confirming the inverse-of-a-product property.
