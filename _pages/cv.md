---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

## Education

**University of Minnesota, Twin Cities** — Ph.D., Electrical and Computer Engineering (Sep 2023 – Jun 2027, expected)
Advisor: [Prof. Chris H. Kim](https://cse.umn.edu/ece/chris-kim) · Area: VLSI, physics-based computing, hardware accelerators

**University of Washington** — M.S., Electrical and Computer Engineering (Sep 2021 – Jun 2023)

**University of Liverpool** — B.Eng., Electrical and Computer Engineering (Sep 2017 – Jun 2021)

---

## Industry Experience

**NVIDIA** — Tegra System Architecture Intern, Westford MA (Summer 2026)

**MediaTek** — ASIC Design Engineer Intern, Chip Design Team, Austin TX (Mar 2023 – Jun 2023)
- Implemented full-chip UPF flow, enabling multi-domain power intent verification.
- Set up and ran clock domain crossing (CDC) and formal equivalence (LEC) checks for sign-off.

**Infineon Technologies** — Digital IC Design Intern, Lynnwood WA (Jan 2023 – Mar 2023)
- Contributed to digital calibration of analog circuits in automotive PSoC.
- Designed a custom low-latency multiplier for calibration, meeting accuracy, efficiency, and area targets.
- Delivered SystemVerilog behavioral models to the analog team for mixed-signal verification.

---

## Research Experience

*Graduate Research Assistant, VLSI Research Laboratory, University of Minnesota (Sep 2023 – Present)*

**All-to-All Coupled Ring Oscillator Ising Solver Chips (TSMC 16nm / 28nm)** (Sep 2023 – Oct 2025)
- Designed and taped out fully programmable all-to-all coupled ring oscillator (RO) Ising solver chips integrating full-custom mixed-signal circuits, on-chip SRAM, and RTL-based digital control.
- Designed programmable memory and control logic for RO coupling weights, local fields, and DCO parameters.
- Implemented in-house SRAM bitcells and periphery; completed full-custom layout, place-and-route, IR drop analysis, and top-level timing sign-off.

**Hardware-Accelerated Ising Decomposer (FPGA Emulation / TSMC 16nm)** (Nov 2024 – Jan 2026)
- Architected an end-to-end hardware pipeline that partitions large Ising/QUBO problems into subproblems for co-processing with Ising solver chips.
- Built a BFS-based partitioning engine in Verilog with dynamic variable clamping and iterative refinement; integrated AXI4-DDR and PCIe host interfaces.
- Verified with RTL–Python co-simulation and SystemVerilog UVM testbenches.

**Diverse Solution Sampling on Physics-Based Ising Hardware** (Jan 2026 – Present)
- Hardware-in-the-loop flow that uses chip stochasticity to return a portfolio of distinct near-optimal solutions, benchmarked against classical samplers on QUBO and SAT instances.

**Scalable CGRA Framework Development** (Mar 2025 – Jul 2025)
- Extended a PyMTL-based hierarchical CGRA to synthesizable RTL, resolved timing bottlenecks, and closed P&R to GDSII with PPA reports.

---

## Silicon Tapeouts and Hardware Artifacts

- **TSMC 28nm all-to-all coupled RO Ising solver chip**: taped out, fabricated, and characterized in silicon.
- **TSMC 16nm all-to-all coupled RO Ising solver chip**: scaled redesign; taped out, fabricated, and characterized in silicon.
- **Ising/QUBO decomposer**: cycle-accurate FPGA emulation of a TSMC 16nm-targeted microarchitecture with AXI4-DDR and PCIe.
- **Hierarchical CGRA test design**: synthesizable RTL through place-and-route to GDSII.

---

## Publications

{% for post in site.publications reversed %}
  {% include archive-single-cv.html %}
{% endfor %}

**Under review**
- C. H. Kim, C. Li, **R. Yin**, X. Li, P. Kreye, H. Lo, T. Islam, "Time-based Couplers using Standard Logic Gates in 28nm and 16nm for Coupled Oscillator Based Ising Solver Chips," *IEEE Journal of Solid-State Circuits (JSSC)*.
- C. H. Kim, P. Kreye, A. Efe, **R. Yin**, et al., "COBIFIVE: A Five-Core Physics-Based Ising Computing Chip," *Nature Electronics*.

**In preparation**
- X. Li\*, **R. Yin**\*, et al., "COBI-Decomposer: A Scalable ASIC Framework for Capacity-Constrained Physics-Based Ising Chips."

---

## Professional Service

- Reviewer, *Future Generation Computer Systems* (Elsevier): 2 manuscripts
- Reviewer, *IEEE International Symposium on Circuits and Systems (ISCAS)*: 6 manuscripts
- Student Member, IEEE

---

## Technical Skills

- **Design & Verification**: Verilog, SystemVerilog, UVM, FPGA emulation
- **Custom / Mixed-Signal VLSI**: full-custom layout, SRAM bitcell and periphery design, SPICE characterization
- **Physical Design**: Cadence Genus/Innovus, IR drop analysis, timing sign-off, Calibre DRC/LVS
- **EDA & Tools**: Synopsys VCS, Verdi, Formality, Xilinx Vivado, Vitis HLS, Quartus, MATLAB
- **Interfaces**: AXI4, PCIe, DDR, QSPI, AHB, RISC-V
- **Programming**: C/C++, Python, PyMTL, Linux/bash
