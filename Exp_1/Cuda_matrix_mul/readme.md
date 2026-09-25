
# CUDA Matrix Multiplication

This folder contains the CUDA implementation of matrix multiplication.

## Implementation

Matrix multiplication is performed using GPU parallelism with CUDA.

## Contents

- CUDA source code
- Output/result screenshots
- Performance results

## CUDA

### CUDA Execution Model

```text
                    CPU / Host
                       │
                 CUDA Kernel Launch
                       │
                       ▼
                  GPU / Device
          ┌─────────────────────────┐
          │        Grid             │
          │ ┌─────┬─────┬─────┐    │
          │ │Block│Block│Block│    │
          │ │  0  │  1  │  2  │    │
          │ ├─────┼─────┼─────┤    │
          │ │Block│Block│Block│    │
          │ │  3  │  4  │  5  │    │
          │ └─────┴─────┴─────┘    │
          └─────────────────────────┘
                       │
                       ▼
               Parallel Threads
                       │
                       ▼
                  Matrix C
```

### Matrix Size vs Execution Time

```text
Matrix Size
     │
     ├── 256 × 256
     ├── 512 × 512
     ├── 1024 × 1024
     └── 2048 × 2048
              │
              ▼
       Execution Time
```
