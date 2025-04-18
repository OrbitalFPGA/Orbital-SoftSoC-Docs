# Orbital SoC: Project Overview

Welcome to the heart of the OrbitalFPGA Soft SoC Project. This file outlines the project architecture, development phases, and integration strategy for building a custom SoC based on the RISC-V RV32I ISA and Wishbone B4 interconnect. To avoid the potentially troublesome terms 'Master' and 'Slave' in the Wishbone bus, they will be replaced by 'Manager' and 'Subordinate' respectively.

## High-Level Architecture
The system consists of modular IP blocks connected via the Wishbone B4 bus. Each module is deisgned to be:
* Reusable and well-documented
* Captabile with other Wishbone-compliant IP
* Validated using software and hardware techniques

## Development Phases
To manage complexity, the project is broken into 5 development phases:

### Phase 1: Core Infrastucture & Bring Up
* Wishbone B4 Subordinate Interface
* FIFO
* UART
* GPIO
* Programmable Timer

### Phase 2: CPU & Bus Infrastructure
* RV32I Proessor Core
* Wishbone Crossbar
* Interrupt Controller

### Phase 3: Communication Peripherals
* SPI Controller
* I2C Controller

### External Memory Support
* SRAM Controller
* SDRAM Controller
* DDR3 Controller
* DMA Engine 

## Design Philosophy 
* Modular: Each IP core is independent and can be tested in isolation
* Wishbone interfaces support reuse across FPGA platforms
* Documented: Every IP block will include interface specs and test strategies
* Testable: Simulations and real hardware bring-up for each module