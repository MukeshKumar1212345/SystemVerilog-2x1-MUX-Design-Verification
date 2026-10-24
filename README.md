# SystemVerilog 2:1 MUX — Design Verification

## Overview
This project demonstrates the design and functional verification of a 4-bit, 2:1 multiplexer using Verilog/SystemVerilog on EDA Playground.

The project was developed as a hands-on learning exercise following a college VLSI workshop conducted by the VLSI First team, which introduced us to Design Verification concepts.

## Design Under Test (DUT)
A 2:1 multiplexer selects one of two 4-bit inputs based on a single select signal.

- `sel = 0`: Output follows `i0`
- `sel = 1`: Output follows `i1`

## Verification Environment
The class-based testbench includes:

- **Transaction:** Stores input and expected-output data.
- **Generator:** Creates randomized input transactions.
- **Driver:** Applies inputs to the DUT.
- **Input Monitor:** Observes inputs and calculates the expected output.
- **Output Monitor:** Observes the DUT output.
- **Scoreboard:** Compares expected and actual outputs.
- **Environment and Test:** Connect and execute the verification components.

## Tools Used
- SystemVerilog
- EDA Playground
- VCS simulator
- EPWave waveform viewer

## Verification Results
The simulation was used to check the MUX functionality by applying input transactions and comparing the expected output against the DUT output.

The waveform demonstrates changes in the input signals, select signal, and output.

## Key Learnings
- Understanding combinational logic and MUX functionality
- Building a class-based SystemVerilog testbench
- Using mailboxes for communication between verification components
- Understanding generators, drivers, monitors, and scoreboards
- Debugging simulations and analysing waveforms

## Acknowledgement
Thanks to the VLSI First team and our college for conducting the workshop and introducing us to Design Verification.

## Project Status
Beginner-level learning project. Further improvements may include additional directed test cases, corner-case verification, and improved testbench synchronization.
