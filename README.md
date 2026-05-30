
# RISC-V Processor Physical Design Flow

## Overview

This project demonstrates the complete RTL-to-GDSII physical design flow of a RISC-V processor core using industry-standard Electronic Design Automation (EDA) tools. The objective is to transform a synthesizable RTL design into a manufacturable physical layout while meeting timing, power, and area constraints.

The project covers all major backend VLSI implementation stages including synthesis, floorplanning, placement, clock tree synthesis (CTS), routing, static timing analysis (STA), and physical verification.

---

## Design Flow

### 1. RTL Design
- Synthesizable RISC-V processor RTL
- Verilog/SystemVerilog implementation
- Functional verification through simulation

### 2. Logic Synthesis
- Conversion of RTL to gate-level netlist
- Standard cell library mapping
- Timing and area optimization
- Constraint-driven synthesis

### 3. Floor Planning
- Core area definition
- Macro and IO placement
- Power planning
- Power and ground ring generation

### 4. Placement
- Standard cell placement
- Congestion analysis
- Timing-driven optimization
- Placement legalization

### 5. Clock Tree Synthesis (CTS)
- Clock network generation
- Clock buffer insertion
- Clock skew minimization
- Timing optimization

### 6. Routing
- Global routing
- Detailed routing
- Design rule compliance
- Signal integrity considerations

### 7. Static Timing Analysis (STA)
- Setup timing analysis
- Hold timing analysis
- Critical path identification
- Timing closure

### 8. Physical Verification
- Design Rule Check (DRC)
- Layout Versus Schematic (LVS)
- Connectivity verification
- Final sign-off checks

---

## Project Structure

```text
RISCV-Physical-Design/
│
├── rtl/
│   ├── riscv_core.v
│   └── testbench.v
│
├── constraints/
│   └── design.sdc
│
├── synthesis/
│   ├── scripts/
│   └── reports/
│
├── floorplan/
│   ├── scripts/
│   └── reports/
│
├── placement/
│   ├── scripts/
│   └── reports/
│
├── cts/
│   ├── scripts/
│   └── reports/
│
├── routing/
│   ├── scripts/
│   └── reports/
│
├── sta/
│   ├── reports/
│   └── timing_analysis/
│
├── verification/
│   ├── drc/
│   └── lvs/
│
└── docs/
    └── flow_documentation.pdf
```

---

## Tools Used

Examples of EDA tools that can be be used for this flow:

- Cadence Innovus
- Cadence Genus
- Synopsys Design Compiler
- Synopsys PrimeTime
- OpenROAD
- OpenLane
- Magic VLSI
- KLayout

---

## Key Outcomes

- Successfully completed RTL-to-GDSII implementation flow.
- Achieved timing closure through iterative optimization.
- Generated routed layout ready for sign-off verification.
- Performed DRC and LVS checks for physical verification.
- Analyzed timing, area, and power metrics throughout the design flow.

---

## Learning Objectives

This project provides hands-on experience in:

- VLSI Backend Design
- Physical Design Methodology
- Timing Closure Techniques
- Clock Tree Optimization
- Physical Verification Flow
- Industry-standard EDA Tool Usage

---

## Future Improvements

- Power optimization using multi-Vt cells
- Clock gating implementation
- Multi-corner multi-mode (MCMM) analysis
- Power integrity analysis (IR Drop)
- Signal integrity and crosstalk optimization
- Full-chip implementation with larger RISC-V cores

---

## Author

Ali Khan

Electronics and Communication Engineering (ECE)

Interested in VLSI Physical Design, RF Engineering, and Embedded Systems.
