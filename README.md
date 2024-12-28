# RISC-V Single Cycle Architecture with CSR

This project implements a **RISC-V processor** using a **single-cycle architecture**. Each instruction is executed in a single clock cycle, and the design includes **Control and Status Registers (CSR)** for managing system-level control and status. The **CSR trap** is hard-wired to handle exceptions.

## Features
- **Single-Cycle Architecture**: Each instruction is completed in one clock cycle.
- **Control and Status Registers (CSR)**: Used for managing system-level control, interrupt handling, and exception processing.
- **Hard-Wired CSR Trap**: Handles exceptions and interrupts directly through the CSR.
- **Basic RISC-V Components**: Includes an ALU, registers, memory, and a control unit.

# Tools used: 
SystemVerilog, VSCode, GTKWave, ModelSim

# Commands:

vlog *.sv  
vsim -c tb_processor -voptargs=+acc -do "run -all"  
gtkwave processor.vcd  
