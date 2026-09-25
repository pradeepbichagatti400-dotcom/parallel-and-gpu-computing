
# MPI Matrix Multiplication

This folder contains the MPI implementation of matrix multiplication.

## Implementation

Matrix multiplication is parallelized using multiple MPI processes.

## Contents

- MPI source code
- MPI communication screenshots
- Output/result screenshots
- Performance results

### MPI Program Flow

```text
                    MPI Program
                        │
                        ▼
                    MPI_Init()
                        │
             ┌──────────┼──────────┐
             │          │          │
             ▼          ▼          ▼
          Process 0   Process 1  Process 2
             │          │          │
             ▼          ▼          ▼
           Data 0     Data 1     Data 2
             │          │          │
             └──────────┼──────────┘
                        │
                   Communication
                        │
                 MPI_Send / MPI_Recv
                        │
                        ▼
                   Final Result
                        │
                        ▼
                  MPI_Finalize()
```

### MPI Process Communication

```text
Process 0 ───── MPI_Send ─────► Process 1
Process 1 ───── MPI_Send ─────► Process 2
Process 2 ───── MPI_Send ─────► Process 0

Process 1 ◄──── MPI_Recv ────── Process 0
```
