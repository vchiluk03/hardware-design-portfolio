# RISC-V SystemC FIR Accelerator (TLM + HLS + Verilog Simulation)

This project documents a SystemC/TLM-based SoC modeling flow where a **RISC-V software stack** interacts with a **DMA-connected FIR accelerator**, with optional **HLS** and **Verilog-level** simulation.

Developed as an academic project, it demonstrates end-to-end understanding from software execution to transaction-level communication and hardware implementation flow.

---

## Project Objective

Build and validate a small accelerator subsystem where:

- a RISC-V program runs through Spike-based simulation,
- data movement is handled through a DMA path,
- a FIR accelerator processes streamed input/coefficient data,
- and the same flow can be evaluated at both SystemC and RTL simulation levels.

---

## Why This Is SoC-Relevant

Yes — this is an **SoC-level understanding project**.

It covers core SoC concepts:

- **HW/SW interaction:** software controls data movement and accelerator execution.
- **Interconnect-level modeling:** transaction flow across SystemC/TLM buses and adapters.
- **Subsystem integration:** CPU model, memory controller, DMA engine, and accelerator connected in one simulation platform.
- **Implementation path:** behavioral model → HLS output → Verilog simulation handoff.

This is not a full production SoC tapeout project, but it is strong SoC-integration and architecture-level experience.

---

## Repository Structure

```text
RISCV-SystemC-FIR-Accelerator/
├── ece720_project2_vchiluk3_report.pdf   # Project report
├── sc/                                   # SystemC model (CPU, DMA, memory, accelerator integration)
├── rocket_sim/                           # RISC-V simulation flow (Spike / emulator integration)
├── hls/                                  # High-level synthesis scripts and outputs
├── vsim/                                 # Verilog simulation executable and setup
├── setup.sh                              # Environment setup script
└── README.md
```

---

## Code Availability

This public project folder keeps documentation and report artifacts only.

- `sc/`, `rocket_sim/`, `hls/`, and `vsim/` contain placeholders in the public version.
- Original source code and scripts are maintained privately.
- Code review access can be requested through the root repository process.

---

## Technical Highlights

- **Modeling:** SystemC transaction-level modeling (TLM).
- **ISA Simulation:** RISC-V Spike-based execution flow.
- **Data Path:** DMA-mediated transfer between memory and accelerator path.
- **Accelerator:** FIR compute pipeline with streamed input/coefficients and packed outputs.
- **Flow Continuity:** support for both SystemC simulation and Verilog simulation using HLS results.

---

## Build and Run (Linux Environment)

```bash
# From project root
source setup.sh

# Build SystemC side
cd sc
make

# Build and run RISC-V simulation flow
cd ../rocket_sim
make
make sim

# Optional: run HLS flow
cd ../hls
make

# Optional: run Verilog simulation flow
cd ../vsim
make
# then switch simulator target in rocket_sim/Makefile as needed
```

Use `make clean` in each subdirectory to remove generated files.

---

## Report

Detailed methodology, architecture, and results are provided in:

- `ece720_project2_vchiluk3_report.pdf`

---

## Skills Demonstrated

- SoC subsystem integration and architecture thinking
- SystemC/TLM modeling and simulation
- RISC-V simulation workflow and performance-awareness
- DMA + accelerator control/data-path understanding
- HLS-to-RTL flow familiarity and simulation handoff
