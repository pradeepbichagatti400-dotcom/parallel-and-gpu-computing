# Parallel and GPU Computing

> **Implementation and Analysis of Matrix Multiplication using Sequential, OpenMP, MPI, and CUDA**

---

## 📌 Overview

This repository contains implementations and experiments for **Parallel and GPU Computing**.

The primary experiment focuses on **Matrix Multiplication** and demonstrates how the same computational problem can be executed using different computing models:

- 🖥️ Sequential Computing
- 🧵 OpenMP Thread Parallelism
- 🔄 MPI Process Parallelism
- ⚡ CUDA GPU Parallelism

The experiment progresses from a single CPU execution flow to highly parallel GPU execution.

---

# 🧭 Computing Model Overview

```mermaid
flowchart TD

    A["Parallel & GPU Computing"]

    A --> B["Matrix Multiplication"]

    B --> C["Sequential"]
    B --> D["OpenMP"]
    B --> E["MPI"]
    B --> F["CUDA"]

    C --> C1["Single CPU Thread"]

    D --> D1["Multiple CPU Threads"]
    D1 --> D2["Shared Memory"]

    E --> E1["Multiple Processes"]
    E1 --> E2["Message Passing"]

    F --> F1["GPU Threads"]
    F1 --> F2["Grid → Blocks → Threads"]

    C1 --> G["Performance Analysis"]
    D2 --> G
    E2 --> G
    F2 --> G
