# HDT2-Paralela


This repository contains a modified version of the classic "Hello World" program using the Message Passing Interface (MPI) for parallel execution.

## Description

In the modified version:
- Processes with even ranks send a "Hello World" message.
- Processes with an odd rank (rank + 1 of the sender) receive the message and print it.

## Prerequisites

Ensure you have an MPI implementation installed, such as [OpenMPI](https://www.open-mpi.org/) or [MPICH](https://www.mpich.org/).

## Compilation

To compile the code, use the `mpicc` compiler:

\```bash
mpicc modified_mpiHello_v2.c -o mpiHello
\```

## Execution

To run the program using `mpirun` or `mpiexec`, specify the number of processes:

\```bash
mpirun -np 4 ./mpiHello
\```

Replace `4` with the desired number of processes.
