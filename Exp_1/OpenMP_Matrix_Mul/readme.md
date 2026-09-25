
# OpenMP Matrix Multiplication

This folder contains the OpenMP implementation of matrix multiplication.

## Implementation

Matrix multiplication is parallelized using OpenMP threads on the CPU.

## Contents

- OpenMP source code
- Output/result screenshots
- Performance results

### OpenMP Thread Distribution

```text
                    Matrix Multiplication
                            │
                            ▼
                       Matrix C
             ┌────────┬────────┬────────┬────────┐
             │        │        │        │        │
             ▼        ▼        ▼        ▼
          Thread 0 Thread 1 Thread 2 Thread 3
             │        │        │        │
             ▼        ▼        ▼        ▼
           Rows      Rows      Rows      Rows
           0–N/4    N/4–N/2  N/2–3N/4  3N/4–N
             │        │        │        │
             └────────┴────────┴────────┴────────┘
                            │
                            ▼
                       Final Matrix
```

### OpenMP Execution Model

```text
OpenMP
  │
  ├── Shared Memory
  │
  ├── Multiple CPU Threads
  │
  ├── #pragma omp parallel
  │
  └── Work distributed among threads
```
