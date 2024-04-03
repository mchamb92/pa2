# Process Scheduling Simulation Tool

This utility simulates process scheduling within an operating system environment, employing various algorithms to illustrate the operations of distinct scheduling strategies.

## Features

- Supports multiple scheduling algorithms:
  - **FCFS (First Come, First Served)**
  - **SRTF (Shortest Remaining Time First)**
  - **RR (Round Robin)**

- Customizable process arrival rates, service times, and quantum intervals.

- Designed for educational purposes to demonstrate scheduling behavior and performance analysis.

## Getting Started

### Prerequisites

- GCC compiler
- Basic understanding of process scheduling concepts

### Compilation

Compile the tool with GCC using the following command:

```bash
gcc -o scheduler scheduler.c -lm

./pa2 <algorithm> <lambda> <mu> <quantum> <max_processes>

Example
./pa2 1 0.25 1.2 3 1500

This will simulate the SRTF scheduling algorithm with a process arrival rate of 0.25 processes/second, an average service time of 1.2 seconds, a Round Robin quantum of 3, and will terminate after 1500 processes have been completed.
