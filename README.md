# GPU Computing

Lecture on GPU computing presented at the [NGMM2026 Summer School](https://www.crs4.it/ngmm2026/) — *Next-Generation Molecular Modeling: Bridging Scales with HPC, AI, and Hybrid Methods*.

Pula, Sardinia, July 27–31, 2026. Organized by CRS4.

The presentation and benchmark data in this repository are dedicated to the public domain under [CC0 1.0 Universal](https://creativecommons.org/publicdomain/zero/1.0/). The CUDA example code is licensed under GPL-3.0-or-later.

## Contents

- Motivation for GPU computing in molecular sciences
- CPU vs GPU architecture
- Heterogeneous computing and the CUDA programming model
- GPU optimization strategies
- GPU-accelerated molecular dynamics and quantum chemistry
- Case study: Amber benchmark of myoglobin on Leonardo (CINECA)

## Repository contents

| Path | Description |
|------|-------------|
| `GPU Computing.pptx` | Lecture slides |
| `LICENSE` | CC0 1.0 Universal (presentation and benchmark data) |
| `amber_benchmark.txt` | Amber benchmark results (myoglobin, 2492 atoms) on Leonardo GPU |
| `benchmark_mpi.txt` | MPI scaling benchmark data for the same system |
| `simple_cuda_program/` | Complete CUDA C vector addition example with Makefile and README |