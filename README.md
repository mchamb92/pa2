Process Scheduling Simulation Tool

This utility offers a dynamic simulation of process scheduling, leveraging various algorithms including FCFS (First Come, First Served), SRTF (Shortest Remaining Time First), and RR (Round Robin) to demonstrate how different scheduling strategies operate.

Getting Started
Compilation
To compile the simulation tool, use gcc by entering the following command:

bash
Copy code
gcc -o scheduler scheduler.c -lm
How to Run
Execute the simulation with required command-line arguments using:

bash
Copy code
./scheduler <algorithm> <lambda> <mu> <quantum> <max_processes>
Parameters:
<algorithm> specifies the scheduling strategy:
0 for FCFS (First Come, First Served)
1 for SRTF (Shortest Remaining Time First)
2 for RR (Round Robin)
<lambda> defines the average rate of process arrivals (processes per second).
<mu> indicates the average service duration (in seconds).
<quantum> sets the quantum interval for the Round Robin algorithm.
<max_processes> denotes the simulation's stopping criterion, based on the total number of processed tasks.
Example Usage
bash
Copy code
./scheduler 1 0.25 1.2 3 1500
This command initiates the simulation utilizing the SRTF scheduling algorithm, featuring an arrival rate of 0.25 processes per second, a service duration of 1.2 seconds, a Round Robin quantum interval of 3, and concludes after completing 1500 tasks.

