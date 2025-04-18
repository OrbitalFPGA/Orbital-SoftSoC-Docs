# Orbital SoC Documentation

Welcome to OrbitalFPGA's Soft SoC project, a public open-source effort to design, implement and document a fully custom RISC-V based soft SoC platform for FPGAs. This repo serces as the centerl documentation hub for the project. 

## 🌌 Project Goals
* Build a completely custom soft SoC based on the RV32I RISC-V core.
* Interconnect all IP blocks via the Wishbone B4 bus standard.
* Create a working toolchain and development environment.

## 🔧 Components
This project consists of multiple modular IP blocks. Each block lives in its own dedicated GitHub repository. A summary of each block can be found in the `docs/` folder with full documentation found in the respective repository. 

The following are the planned components
* Wishbone B4 Servent Interface
* First-In-First-Out
* UART
* GPIO
* Programmable timer
* RV32I Processor
* Memory controllers

## Repostiory Structure

```
orbital-softsoc-docs/
├── README.md                 # Project overview (this file)
├── docs/                     # Documentation for each IP block
│   ├── 00_overview.md
│   └── ...
├── diagrams/                 # System diagrams, memory maps, etc.
│   ├── soc_block_diagram.drawio
│   ├── wishbone_crossbar.svg
│   └── memory_map.png
└── links/                    # External repo index, datasheets, etc.
    ├── repo_index.md
    └── references.md
```

## Stay Updated
Follow [@OrbitalFPGA](https://github.com/OrbitalFPGA) and star this repo to stay updated on progress.
