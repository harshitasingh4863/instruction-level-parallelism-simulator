# Instruction-Level Parallelism Simulator

## About the Project

This project is a Python-based simulation of Instruction-Level Parallelism (ILP). It demonstrates how independent instructions can be executed in parallel to reduce the total number of execution cycles.

The project compares sequential instruction execution with parallel execution and calculates the resulting speedup and efficiency.

## Objectives

* Understand the concept of Instruction-Level Parallelism.
* Identify dependencies between instructions.
* Simulate sequential instruction execution.
* Simulate parallel execution of independent instructions.
* Compare execution cycles.
* Calculate ILP speedup and efficiency.

## Technologies Used

* Python 3
* Visual Studio Code
* GitHub

## How It Works

The simulator uses a set of simple register-based instructions.

For example:

```text
I1: R1 = R2 + R3
I2: R4 = R5 + R6
I3: R7 = R1 + R4
```

I1 and I2 are independent and can execute in parallel.

I3 depends on the results of I1 and I2, so it must wait until both instructions are completed.

## Execution Modes

### Sequential Execution

Instructions are executed one after another.

```text
I1 → I2 → I3 → I4 → I5 → I6
```

### ILP Execution

Independent instructions are executed in the same cycle.

```text
Cycle 1: I1, I2, I4, I6
Cycle 2: I3
Cycle 3: I5
```

## Performance

The simulator calculates:

```text
Speedup = Sequential Cycles / ILP Cycles
```

ILP can reduce the number of cycles required when multiple instructions are independent.

## How to Run

Clone the repository:

```bash
git clone <repository-url>
```

Open the project folder:

```bash
cd instruction-level-parallelism-simulator
```

Run the program:

```bash
python ilp_simulator.py
```

## Project Structure

```text
instruction-level-parallelism-simulator/
│
├── ilp_simulator.py
├── README.md
├── documentation/
└── screenshots/
```

## Conclusion

The simulation demonstrates that Instruction-Level Parallelism can improve processor performance by executing independent instructions simultaneously. However, dependencies between instructions can limit the amount of parallelism available.

## Author

Harshita Singh

B.Tech CSE (AIML)
SGT University, Gurugram
