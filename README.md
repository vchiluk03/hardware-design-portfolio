# Hardware Design & Verification Portfolio

Portfolio of **ASIC Design, RTL Verification, and Computer Microarchitecture** projects by **Vishnuvardhan Chilukoti**.

[![Domain](https://img.shields.io/badge/Domain-Digital%20Design%20%7C%20Verification-blue)](#)
[![Focus](https://img.shields.io/badge/Focus-UVM%20%7C%20SystemVerilog%20%7C%20C%2B%2B-informational)](#)
[![Status](https://img.shields.io/badge/Portfolio-Active-success)](#)

This repository is a curated showcase of project documentation, architecture artifacts, validation results, and methodology notes from advanced hardware-focused work.

---

## Portfolio Snapshot

- **Primary Focus:** Functional verification (UVM-style), RTL architecture, and performance-oriented microarchitecture simulation.
- **Core Domains:** Bus protocols (Wishbone/I²C), decode/control logic verification, memory hierarchy, branch prediction, and out-of-order execution.
- **Methodology:** Structured test planning, layered environments, coverage-driven closure, and reproducible simulation/synthesis flows.

---

## Featured Projects

| Project | Area | Highlights | Link |
|---|---|---|---|
| **I²C Multi-Bus Master Verification** | ASIC Verification | Wishbone↔I²C bridge verification with layered testbench, assertions, regression, and coverage closure | [I2CMB-Controller-Verification](./I2CMB-Controller-Verification) |
| **LC-3 Decode Unit UVM Verification** | UVM / CPU Verification | Predictor + scoreboard architecture for decode correctness and control-signal validation | [LC3-CPU-Decode-UVM](./LC3-CPU-Decode-UVM/decode_unit_uvm) |
| **Interrupt Controller Design & Verification** | RTL Design + DV | Parameterized interrupt arbitration with APB-style configurability and task-based verification | [Interrupt-Controller-Design-Verification](./Interrupt-Controller-Design-Verification) |
| **Microarchitecture Simulations** | Computer Architecture | C++ simulators for cache hierarchy, branch prediction, and out-of-order superscalar behavior | [Microarchitecture-Simulations](./Microarchitecture-Simulations) |
| **Transformer Attention Accelerator** | ASIC RTL + Synthesis | FSM-controlled scaled dot-product attention datapath with SRAM-based architecture and synthesis analysis | [Transformer-Attention-Accelerator](./Transformer-Attention-Accelerator) |

---

## Technical Competencies

- **HDL & Verification:** SystemVerilog, Verilog, UVM-style environments, assertions, scoreboards, predictors, constrained-random and directed testing.
- **Protocols & Interfaces:** I²C, Wishbone, APB-style register access, memory-mapped control paths.
- **Architecture & Performance:** Cache hierarchy analysis, branch predictor design (Bimodal/Gshare/Hybrid), Tomasulo-style out-of-order modeling.
- **Tooling:** Questa/ModelSim, Makefile-based automation, Synopsys Design Compiler, waveform/debug workflows.
- **Programming:** C++ (microarchitecture simulators), Python (input/workflow scripting).

---

## Repository Content Policy

To uphold academic integrity and responsible sharing practices:

- **Included:** Documentation, reports, figures, waveform snapshots, setup notes, and non-sensitive artifacts.
- **Restricted:** Original graded source files and selected scripts are not publicly exposed in raw form.

This portfolio is intentionally structured for **technical review and discussion** while respecting coursework and sharing constraints.

---

## Code Access for Recruiting / Interviews

If your evaluation requires code-level review, submit a request using:

**Code Access Request Form**  
https://github.com/vchiluk03/hardware-design-portfolio/issues/new?template=code_access_request.yml&title=Code%20Access%20Request

### Review Process

1. Submit the request with role/company context.
2. Requests are reviewed manually.
3. Approved access is provided in a **read-only format** (for example: PDF snapshot or time-limited archive).

> Direct collaborator access to private repositories is not granted.

---

## Quick Navigation

- [I2CMB Verification README](./I2CMB-Controller-Verification/README.md)
- [LC-3 Decode UVM README](./LC3-CPU-Decode-UVM/decode_unit_uvm/README.md)
- [Interrupt Controller README](./Interrupt-Controller-Design-Verification/README.md)
- [Microarchitecture Simulations README](./Microarchitecture-Simulations/README.md)
- [Attention Accelerator README](./Transformer-Attention-Accelerator/README.md)

---

## Contact

**Vishnuvardhan Chilukoti**  
Email: **vchiluk3@gmail.com**


