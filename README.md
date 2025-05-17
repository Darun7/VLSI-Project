# VLSI-Project
# 16-Input Bit Mapping-Based OFDM Implementation on FPGA

This repository contains the design, simulation, and implementation of an Orthogonal Frequency Division Multiplexing (OFDM) transceiver on an FPGA platform using Verilog HDL. The system is designed to support high data rate communication using 16-QAM modulation and an 8-point IFFT/FFT-based architecture.

## Project Overview

- **Title**: 16-Input Bit Mapping-Based OFDM Implementation on FPGA for High Data Rate Communication
- **Platform**: Xilinx ZedBoard (Zynq xc7z020clg484-1)
- **Tool Used**: Xilinx Vivado 2024.1.2
- **Language**: Verilog HDL
- **Objective**: To implement a complete OFDM transceiver using 16-QAM, symbol modulation, IFFT/FFT, cyclic prefixing, and zero-padding to enhance data transmission efficiency and robustness.

## Transmitter Architecture

1. Bit Stream Generator
2. 16-QAM Modulator
3. Symbol Modifier
4. Zero-Padder
5. IFFT (8-point, 16-bit)
6. Cyclic Prefixing
7. Serializer

## Receiver Architecture

1. Inverse Cyclic Prefixing
2. FFT (8-point, 16-bit)
3. Inverse Zero-Padder
4. Inverse Symbol Modifier
5. QAM Demapping

## Simulation and Results

- Both transmitter and receiver were simulated and verified in Vivado.
- Successfully recovered all 16 possible 4-bit sequences at the receiver end.
- Demonstrated robustness to inter-symbol interference through cyclic prefixing.

## Files Included

- `open lab paper with plag report.pdf`: Contains detailed project documentation and plagiarism report.

## References

1. IEEE and research publications on OFDM and FPGA implementation
2. Prior works using Verilog HDL for signal processing systems

## Authors

- **Pugalbharani N** – ch.en.u4ece22034@ch.students.amrita.edu  
- **Darun Eiswar S** – ch.en.u4ece22015@ch.students.amrita.edu  
- **Mentor**: Ms. Sakkthi Saranya.
