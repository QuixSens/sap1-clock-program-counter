# Clock & Program Counter — SAP-1 Style 8-bit Computer

Design and implementation of the clock and program counter (PC) modules for an SAP-1-style 8-bit computer, responsible for instruction sequencing and system-wide timing synchronization across all modules — MAR, RAM, registers, ALU, and the shared 8-bit bus.

## Key Specifications

| Parameter | Value |
|---|---|
| Clock IC | 555 Timer (astable, monostable, bistable modes) |
| Program Counter | 4-bit, built with 74LS161 synchronous counters |
| Bus Interface | 74LS245 transceiver |
| Verification | LED-based functional testing |

## Design Architecture

- **Multi-mode clock circuit** — 555 timer configured across astable, monostable, and bistable modes to generate and control system timing
- **4-bit program counter** — built using 74LS161 synchronous counters for instruction address sequencing
- **Bus interfacing** — 74LS245 transceiver manages PC-to-system-bus communication
- **System integration** — clock and PC integrated with MAR, RAM, registers, ALU, and the common 8-bit bus

## Verification & Debugging

Clocking, counting, and bus behavior were verified using LED indicators at each stage, with systematic debugging performed to resolve timing and interfacing issues during system-level integration.

## Repository Structure

```
├── docs/
│   └── lab_report.pdf
├── schematics/
│   ├── clock_circuit.png
│   └── program_counter.png
├── images/
│   └── integration_testing/
└── README.md
```

## Tools & Components

`555 Timer` `74LS161` `74LS245` `Breadboard Prototyping` `LED-based Verification`

*Solo project — Electronics Design Lab (ED214), Semester III.*