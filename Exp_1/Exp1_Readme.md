
# Experiment 1 - Matrix Multiplication

This experiment implements matrix multiplication using different parallel computing approaches:

- Sequential Matrix Multiplication
- OpenMP Matrix Multiplication
- MPI Matrix Multiplication
- CUDA Matrix Multiplication


Same matrix multiplication problem → four different execution models

                    Matrix Multiplication
                            │
                            ▼
                  A × B = C
                            │
          ┌─────────────────┼─────────────────┐
          │                 │                 │
          ▼                 ▼                 ▼
     Sequential          OpenMP             MPI
       CPU               Threads          Processes
          │                 │                 │
          └─────────────────┼─────────────────┘
                            │
                            ▼
                          CUDA
                           GPU
                            │
                            ▼
                    Performance Analysis


## Performance Analysis

```text
Execution Time
      │
      ├── Sequential
      ├── OpenMP
      ├── MPI
      └── CUDA

Resource Utilization
      │
      ├── CPU
      ├── Threads
      ├── Processes
      └── GPU
```



Execution Time (ms)

Sequential  ████████████████████
OpenMP      ███████████
MPI         ████████
CUDA        ███
