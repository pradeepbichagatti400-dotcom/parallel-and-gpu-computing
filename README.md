# Parallel and GPU Computing

Programs, experiments, implementations, and performance analysis for
Parallel and GPU Computing.

---

## 1. Overview

This repository demonstrates how the **same computational problem** can be
implemented using different execution models:

- Sequential Computing
- OpenMP-based CPU Parallelism
- MPI-based Process Parallelism
- CUDA-based GPU Parallelism

The primary problem considered in Experiment 1 is **Matrix Multiplication**.

The objective is to understand how computation changes when moving from
single-threaded execution to CPU parallelism, process-based parallelism,
and GPU parallelism.

---

## 2. Experiment 1 — Matrix Multiplication

Matrix multiplication is used as a common problem for all four approaches.

Given two matrices:

```text
A × B = C
