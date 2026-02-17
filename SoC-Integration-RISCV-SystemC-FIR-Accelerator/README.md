# RISC-V SystemC FIR Accelerator (SoC Integration)

This project presents a **SystemC/TLM SoC integration flow** where a RISC-V software stack drives a **DMA-connected FIR accelerator**, with continuity into **HLS** and **Verilog simulation**.

Built as an academic SoC modeling project, it demonstrates end-to-end understanding across software execution, interconnect transactions, hardware acceleration, and simulation handoff.

## Objective

Design and validate a small accelerator subsystem in which:

- RISC-V software runs through Spike/emulation flow,
- DMA moves data between memory and the accelerator,
- FIR computation executes on the accelerator path,
- and behavior can be studied at both SystemC and RTL levels.

## SoC Integration Scope

This project focuses on practical SoC-integration concepts:

- **HW/SW interaction:** software-triggered data movement and accelerator execution.
- **Interconnect-level modeling:** transaction flow through SystemC/TLM components.
- **Subsystem composition:** CPU model, memory, DMA, and FIR accelerator in one platform.
- **Implementation continuity:** behavioral model to HLS/Verilog simulation flow.

## Repository Structure

```text
SoC-Integration-RISCV-SystemC-FIR-Accelerator/
├── ece720_project2_vchiluk3_report.pdf
├── sc/           # SystemC/TLM subsystem modeling
├── rocket_sim/   # RISC-V software/simulation flow
├── hls/          # High-level synthesis flow artifacts
├── vsim/         # Verilog simulation setup
├── setup.sh
└── README.md
```

## Public Portfolio Notes

This public project folder is a portfolio-facing version.

- Documentation/report artifacts are preserved for review.
- Some implementation files are intentionally withheld from this public copy.
- Code access requests are handled via the public repository request form:

https://github.com/vchiluk03/hardware-design-portfolio/issues/new?template=code_access_request.yml&title=Code%20Access%20Request

## Technical Highlights

- SystemC/TLM transaction modeling for SoC communication paths.
- RISC-V execution flow integration with accelerator control.
- DMA-based streaming data path to FIR compute block.
- HLS/RTL simulation handoff awareness in one project flow.

## Build Flow Reference (Linux)

```bash
# Environment setup
source setup.sh

# SystemC model
cd sc && make

# RISC-V simulation
cd ../rocket_sim && make && make sim

# Optional HLS flow
cd ../hls && make

# Optional Verilog simulation
cd ../vsim && make
```

Use `make clean` within each subdirectory as needed.

## Report

Project report:

- `ece720_project2_vchiluk3_report.pdf`

## Skills Demonstrated

- SoC subsystem integration and architecture-level reasoning
- SystemC/TLM modeling and simulation workflow
- RISC-V software/hardware co-simulation understanding
- DMA and accelerator control/data-path integration
- HLS-to-RTL flow awareness
