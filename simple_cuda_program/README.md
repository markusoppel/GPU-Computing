# Simple CUDA Vector Addition

A minimal CUDA C program that adds two vectors on the GPU.

Copyright (C) 2026 Markus Oppel, University of Vienna  
License: GPL-3.0-or-later

## Prerequisites

- NVIDIA GPU with CUDA support
- [CUDA Toolkit](https://developer.nvidia.com/cuda-downloads) (includes `nvcc`)

## Compile and Run

```bash
make          # compile
make run      # compile and run
./vector_add  # run manually
make clean    # remove binary
```

## What it does

Allocates two float arrays `a` and `b` on the host, copies them to the GPU,
launches a kernel (`add`) that computes `c[i] = a[i] + b[i]` for each element
in parallel, copies the result back, and prints the first ten values.

The grid launch uses 256 threads per block and enough blocks to cover all `N`
elements (`N = 2^20`).