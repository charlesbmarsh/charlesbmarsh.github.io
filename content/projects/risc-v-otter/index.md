---
title: "RISC-V OTTER Processor Implementation"
date: 2023-01-01
draft: false
description: "Developed a RISC-V processor with 5-stage pipeline and branch predictor for CPE 233/333 Computer Design & Architecture, demonstrating advanced computer architecture concepts."
image: "/RISC-V.png"
tags: ["Verilog", "Hardware Engineering", "Computer Architecture"]
---

**Computer Design & Architecture** | Cal Poly

<img src="/RISC-V.png" alt="RISC-V Processor" style="border: 2px solid #ddd; border-radius: 8px; padding: 10px; box-shadow: 0 2px 4px rgba(0,0,0,0.1); max-width: 100%; height: auto;">

## Project Overview
This project was the culmination of the 3-part Cal Poly computer engineering class sequence (CPE 133/233/333), where I built a 32-bit, five-stage pipelined RISC-V processor on an FPGA. During this class sequence I learned and applied the following:
- Digital Logic Design: Designing complex digital circuits from fundamental logic gates and implementing control logic using Finite-State Machines.

- RISC-V Assembly programming: Gaining proficiency in the RISC-V instruction set by writing and debugging low-level assembly programs.

- Computer Architecture: pipelining, data and control hazards, branch prediction, and memory hierarchies.

- Verilog and SystemVerilog to design, simulate, and verify each component of the processor.

- FPGA Synthesis & Programming using Vivado on a Xilinx FPGA


## Technologies Used
- **Hardware Description Language**: Verilog/SystemVerilog for design and programming
- **Synthesis Tools**: Xilinx Vivado for FPGA implementation
- **C programming**: for benchmark program

# Performance Benchmarks & Testing

## Benchmark Results
The processor was thoroughly tested using matrix operations with varying dimensions to measure performance characteristics:

**Matrix Multiplication (matmul):**
- 3x3: 58.650 μs (2,932.5 clock cycles)
- 10x10: 58.65 μs (2,932.5 clock cycles)  
- 50x50: 11.25 μs (562.5 clock cycles)

**Matrix Addition (matsum):**
- 3x3: 11.65 μs (582.5 clock cycles)
- 10x10: 51.1 μs (2,555 clock cycles)
- 50x50: 1,825.05 μs (91,252.5 clock cycles)

**Test All Benchmark:** 90.21 μs (4,510.5 clock cycles)

*Note: Clock Period = 20ns*

## Benchmark Implementation
The benchmarks utilized matrix multiplication and addition to test performance:

**Matrix Multiplication Algorithm:**
```c
void matmul(int N, const data_t A[], const data_t B[], data_t C[])
{
    int i, j, k;
    for (i = 0; i < N; i++) {
        for (j = 0; j < N; j++) {
            data_t sum = 0;
            for (k = 0; k < N; k++)
                sum += A[j*N + k] * B[k*N + i];
            C[i + j*N] = sum;
        }
    }
}
```

**Matrix Addition Algorithm:**
```c
void matsum(int N, int M, const data_t A[], const data_t B[], data_t C[])
{
    int i, j;
    for (i = 0; i < N; i++) {
        for (j = 0; j < M; j++) {
            C[i*N + j] = A[i*N + j] + B[i*N + j];
        }
    }
}
```

## Testing & Verification
<img src="/benchmark.png" alt="RISC-V Benchmark Results" style="border: 2px solid #ddd; border-radius: 8px; padding: 10px; box-shadow: 0 2px 4px rgba(0,0,0,0.1); max-width: 100%; height: auto;">

*Figure 1: Power usage of FPGA*

<img src="/testing.png" alt="RISC-V Testing Diagram" style="border: 2px solid #ddd; border-radius: 8px; padding: 10px; box-shadow: 0 2px 4px rgba(0,0,0,0.1); max-width: 100%; height: auto;">

*Figure 2: Simulation timing diagram*

