
# Problem 03 – When Can Matrices Be Multiplied?

## Solution

The matrix sizes are:

- A: 2 × 3
- B: 3 × 4
- C: 4 × 2
- D: 2 × 2

Matrix multiplication is possible when the number of columns of the first matrix equals the number of rows of the second matrix.

### 1. AB

A is 2 × 3 and B is 3 × 4.

Since 3 = 3, the multiplication is defined.

The result has size **2 × 4**.

### 2. BA

B is 3 × 4 and A is 2 × 3.

Since 4 ≠ 2, the multiplication is not defined.

### 3. BC

B is 3 × 4 and C is 4 × 2.

Since 4 = 4, the multiplication is defined.

The result has size **3 × 2**.

### 4. CB

C is 4 × 2 and B is 3 × 4.

Since 2 ≠ 3, the multiplication is not defined.

### 5. AC

A is 2 × 3 and C is 4 × 2.

Since 3 ≠ 4, the multiplication is not defined.

### 6. CA

C is 4 × 2 and A is 2 × 3.

Since 2 = 2, the multiplication is defined.

The result has size **4 × 3**.

### 7. AD

A is 2 × 3 and D is 2 × 2.

Since 3 ≠ 2, the multiplication is not defined.

### 8. DA

D is 2 × 2 and A is 2 × 3.

Since 2 = 2, the multiplication is defined.

The result has size **2 × 3**.

### Final Answer

| Product | Defined? | Result Size |
|---------|----------|-------------|
| AB | Yes | 2 × 4 |
| BA | No | — |
| BC | Yes | 3 × 2 |
| CB | No | — |
| AC | No | — |
| CA | Yes | 4 × 3 |
| AD | No | — |
| DA | Yes | 2 × 3 |
