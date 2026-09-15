# instruction-level-parallelism-simulator
A Python-based simulation of Instruction-Level Parallelism comparing sequential and parallel instruction execution.
# Instruction-Level Parallelism Simulator

## About the Project

This project is a Python-based simulation of Instruction-Level Parallelism (ILP).

The simulator compares sequential instruction execution with parallel execution of independent instructions.

## Objectives

- Understand Instruction-Level Parallelism.
- Identify instruction dependencies.
- Simulate sequential execution.
- Simulate parallel execution.
- Calculate execution cycles.
- Calculate speedup and efficiency.

## Technologies Used

- Python
- Visual Studio Code
- GitHub

## How It Works

The simulator uses a set of register-based instructions.

Example:

I1: R1 = R2 + R3

I2: R4 = R5 + R6

I3: R7 = R1 + R4

I1 and I2 are independent and can execute in parallel.

I3 depends on the results of I1 and I2.

## How to Run

Open the project in Visual Studio Code.

Run the following command:

```bash
python ilp_simulator.py
