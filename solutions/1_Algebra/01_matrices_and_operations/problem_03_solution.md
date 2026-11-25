### Exercise 3. When Can Matrices Be Multiplied?

**Problem:**

The matrix sizes are

$$
A_{2\times3},\qquad B_{3\times4},\qquad C_{4\times2},\qquad D_{2\times2}.
$$

For the products

$$
AB,\ BA,\ BC,\ CB,\ AC,\ CA,\ AD,\ DA
$$

determine whether they are defined. If so, state the size of the result. Justify each decision using the dimension compatibility condition.

---

## Solution

### Dimension Compatibility Rule for Multiplication

Two matrices $X$ and $Y$ can be multiplied in the order $XY$ if and only if the number of columns in $X$ equals the number of rows in $Y$. If $X$ is of size $m \times n$ and $Y$ is of size $n \times p$, then the product $XY$ is defined and has the size $m \times p$.

### Analysis of Each Product

* **$AB$ ($A_{2\times3}$ and $B_{3\times4}$):**
  * The number of columns of $A$ ($3$) matches the number of rows of $B$ ($3$).
  * **Status:** Defined.
  * **Size of result:** $2 \times 4$.

* **$BA$ ($B_{3\times4}$ and $A_{2\times3}$):**
  * The number of columns of $B$ ($4$) does not match the number of rows of $A$ ($2$).
  * **Status:** Undefined.

* **$BC$ ($B_{3\times4}$ and $C_{4\times2}$):**
  * The number of columns of $B$ ($4$) matches the number of rows of $C$ ($4$).
  * **Status:** Defined.
  * **Size of result:** $3 \times 2$.

* **$CB$ ($C_{4\times2}$ and $B_{3\times4}$):**
  * The number of columns of $C$ ($2$) does not match the number of rows of $B$ ($3$).
  * **Status:** Undefined.

* **$AC$ ($A_{2\times3}$ and $C_{4\times2}$):**
  * The number of columns of $A$ ($3$) does not match the number of rows of $C$ ($4$).
  * **Status:** Undefined.

* **$CA$ ($C_{4\times2}$ and $A_{2\times3}$):**
  * The number of columns of $C$ ($2$) matches the number of rows of $A$ ($2$).
  * **Status:** Defined.
  * **Size of result:** $4 \times 3$.

* **$AD$ ($A_{2\times3}$ and $D_{2\times2}$):**
  * The number of columns of $A$ ($3$) does not match the number of rows of $D$ ($2$).
  * **Status:** Undefined.

* **$DA$ ($D_{2\times2}$ and $A_{2\times3}$):**
  * The number of columns of $D$ ($2$) matches the number of rows of $A$ ($2$).
  * **Status:** Defined.
  * **Size of result:** $2 \times 3$.




