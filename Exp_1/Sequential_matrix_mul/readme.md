
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



Matrix A              Matrix B              Matrix C
┌───────┐             ┌───────┐             ┌───────┐
│ a a a │             │ b b b │             │ c c c │
│ a a a │     ×       │ b b b │     =       │ c c c │
│ a a a │             │ b b b │             │ c c c │
└───────┘             └───────┘             └───────┘
                                              
                     C[i][j] =
              Σ A[i][k] × B[k][j]

