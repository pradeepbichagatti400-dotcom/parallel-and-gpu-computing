
# Sequential Matrix Multiplication

This folder contains the sequential implementation of matrix multiplication.

## Implementation

Matrix multiplication is performed using the traditional sequential approach without parallel processing.

## Contents

- Sequential source code
- Output/result screenshots
- Performance results

## Purpose

This implementation serves as the baseline for comparing sequential execution with OpenMP, MPI, and CUDA implementations.

### Matrix Multiplication

```text
Matrix A              Matrix B              Matrix C
┌───────┐             ┌───────┐             ┌───────┐
│ a a a │             │ b b b │             │ c c c │
│ a a a │     ×       │ b b b │     =       │ c c c │
│ a a a │             │ b b b │             │ c c c │
└───────┘             └───────┘             └───────┘

                     C[i][j] =
              Σ A[i][k] × B[k][j]
```
### Sequential Matrix Multiplication

```text
Start
  │
  ▼
Read Matrix A and B
  │
  ▼
Initialize Matrix C
  │
  ▼
For each row i
  │
  ▼
  For each column j
      │
      ▼
    For each k
      │
      ▼
 C[i][j] += A[i][k] × B[k][j]
      │
      ▼
Repeat until complete
  │
  ▼
Display Result
```
