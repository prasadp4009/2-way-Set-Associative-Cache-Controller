# 2-Way Set Associative Cache Controller

Synthesizable and Parameterized Cache Controller in Verilog

This repository contains the RTL (Register Transfer Level) code for a 2-Way Set Associative Cache Controller, as discussed in the accompanying [report](https://github.com/prasadp4009/2-way-Set-Associative-Cache-Controller/blob/master/Report.pdf).

## Project Overview

The project implements a 2-Way Set Associative Cache system. Key features include:

- **Bidirectional Data Bus**: The data bus for both the CPU and Main Memory are bidirectional, controlled using Write CPU and Write Mem signals.
- **Memory Access Protocol**: Memory uses an active HIGH ready signal to follow data access and write protocol.
- **CPU Operation**: The CPU halts operation and keeps address and data lines active when 'stall_cpu' gets and stays high. The CPU reads the data in the next clock cycle when 'stall_cpu' gets low.
- **State Management**: The system operates in various states such as IDLE, READ, WRITE, READMM, WAITFORMM, UPDATEMM, UPDATECAHE, each with specific behaviors.

## Documentation

The repository includes a detailed [report](https://github.com/prasadp4009/2-way-Set-Associative-Cache-Controller/blob/master/Report.pdf) with flow diagrams for read and write operations, state descriptions, and timing diagrams for different scenarios.

## Authors

This project is developed by Prasad Pandit & Radhika Mandlekar.
