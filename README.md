# AHB-to-APB Bridge — Verilog RTL Design

## Overview

This project implements a modular RTL-based bridge between the AMBA AHB
(Advanced High-performance Bus) and APB (Advanced Peripheral Bus)
protocols using Verilog HDL.

The bridge translates AHB transactions into APB transactions, allowing
an AHB-based system to communicate with APB-based peripheral interfaces.

## Architecture

The design is organized into separate RTL modules for the AHB and APB
interfaces and the bridge control logic.

## Main RTL Blocks

- **AHB Master** — Generates AHB-side address, control, and data signals.
- **AHB Slave Interface** — Receives and processes AHB transactions.
- **APB Controller** — Controls the APB transfer sequence.
- **APB Interface** — Handles APB-side address, control, and data signals.
- **Bridge Top** — Integrates the AHB and APB components into the complete bridge.

## Key Features

- Verilog RTL implementation
- Modular AMBA bus architecture
- AHB-to-APB transaction conversion
- FSM-based control logic
- Address decoding
- Read and write transfer handling
- Separate AHB and APB interface modules
- Simulation-based functional verification

## Project Structure

```text
AHB-to-APB-Bridge-Verilog/
│
├── rtl/
│   ├── AHB_Master.v
│   ├── AHB_Slave_Interface.v
│   ├── APB_Controller.v
│   ├── APB_Interface.v
│   └── bridge_top.v
│
├── docs/
│   └── AHB-to-APB-Bridge project report.pdf
│
├── block diagrams and outputs/
│   └── Simulation and block diagram outputs
│
└── README.md
