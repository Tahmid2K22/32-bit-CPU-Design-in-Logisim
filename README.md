# 32-bit-CPU-Design-in-Logisim


This project simulates a complete 32-bit CPU architecture in **Logisim**, built from scratch to demonstrate core concepts of computer architecture and CPU operation. It implements a custom instruction set, manages control flow, and supports stack-based memory operations.

Developer
- **Name:** Tahmid Hossain Chowdhury Mahin  


##Components
- **MAR (Memory Address Register)**: Holds the address to access from memory.
- **MBR (Memory Buffer Register)**: Temporarily stores data during memory-CPU transfers.
- **PC (Program Counter)**: Tracks the next instruction's address.
- **IR (Instruction Register)**: Holds the current executing instruction.
- **AC (Accumulator)**: Stores temporary data for ALU operations.
- **CU (Control Unit)**: Manages the fetch-decode-execute cycle.
- **ALU (Arithmetic Logic Unit)**: Performs bitwise and arithmetic operations.

## 📜 Supported Instructions
- `ADD`, `AND`, `STORE`, `LOAD`, `BUN`, `BSB`, `ISZ`, `HALT`
- **Special Instructions:**
  - `MOD`: Modulus via repeated subtraction.
  - `SWAP`: Swaps AC value with memory.
  - `DELAY`: Adds wait cycles using memory-defined timing.
  - `PUSH` / `POP`: Stack operations using the end of memory as the stack pointer.

## 🔁 Fetch-Decode-Execute Cycle
The control unit executes each instruction using a classic CPU cycle:
1. **Fetch** – Retrieve instruction from memory.
2. **Decode** – Interpret the instruction type.
3. **Execute** – Carry out operation via CU/ALU/memory.

## 🧪 Stack Implementation
- Uses the last address of RAM as the initial stack pointer.
- Supports 32-bit data push and pop operations.

## 📚 References
- _Digital Logic and Computer Design_ by M. Morris Mano
- University Lab Materials & Slides


