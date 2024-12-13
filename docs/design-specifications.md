# Detailed design documents and diagrams

## Processor Design

![Processor Macro Design Diagram](/media/diagrams/processor-macro-design-diagram.png)

### Specifications

#### General Overview
- **Processor Type**: Custom, 16-bit processor
- **Architecture**: Von Neumann architecture (shared memory for instructions and data)
- **Clock Speed**: 1-10 MHz (depending on design and hardware limitations)

#### CPU Specifications
- **Data Bus Width**: 16 bits (can process 16 bits of data at a time)
- **Address Bus Width**: 16 bits (up to 64KB of addressable memory)

#### Registers
- **General-Purpose Registers**: 8 registers (R0 to R7), each 16 bits wide
- **Special-Purpose Registers**:
  - **PC (Program Counter)**: 16 bits, holds the address of the next instruction
  - **IR (Instruction Register)**: 16 bits, stores the current instruction
  - **SR (Status Register)**: 16 bits, holds flags (Zero, Carry, Overflow, Negative)

#### ALU (Arithmetic Logic Unit)
- **Width**: 16 bits (supports 16-bit arithmetic and logical operations)
- **Operations Supported**: Addition, subtraction, AND, OR, XOR, NOT
- **Flags**: Updates the **SR (Status Register)** based on the results of operations

#### Control Unit (CU)
- **Function**: Decodes instructions and generates control signals to manage the operation of the processor
- **Control Signals**: Manages data flow between **Registers**, **ALU**, and **RAM**

#### Clock
- **Clock Speed**: 1-10 MHz (controls synchronization of the processor's operations)
- **Timing**: The **Clock** triggers the fetch-decode-execute cycle of instructions

#### Memory
- **RAM**: 64KB (addressable with the 16-bit address bus)
  - **Why 64KB is the Maximum**: The **64KB limit** comes from the **16-bit address bus**, which can address **2^16** (64KB) of memory. The **address bus width** is 16 bits, meaning it can access a maximum of 64KB of memory. While larger amounts of memory can be implemented using **paging** or **bank-switching** techniques, this design limits the **addressable space** to **64KB** as a starting point.
  - **Read/Write Operations**: Managed by the **Control Unit (CU)**, which controls when data is read from or written to **RAM**.
