# 8-Bit ALU Simulator

An interactive, standalone HTML/JavaScript simulator for an **8-Bit Arithmetic Logic Unit (ALU)** based on the Logisim logic diagram.

## Files

- `index.html` — Self-contained 8-bit ALU web simulator (no server or build step required)
- `alu_diagram.png` — Original 8-bit ALU logic diagram

## Features

- **8-Bit Operands (`A` and `B`)**:
  - Clickable 8-bit binary switches (`D7`–`D0`)
  - Live-synced **Decimal** input fields (`0–255` unsigned, `−128–127` signed)
  - Range sliders and `−` / `+` step buttons
- **4 Parallel Arithmetic Operations (2-Bit Opcode + 4:1 MUX)**:
  - `00` **ADD (`A + B`)** — outputs 8-bit sum and `Cout` (Carry Out)
  - `01` **SUB (`A − B`)** — outputs 8-bit difference and `borrowout`
  - `10` **MUL (`A × B`)** — outputs lower 8 bits and full 16-bit product details
  - `11` **DIV (`A ÷ B`)** — outputs 8-bit quotient and 8-bit `Remainder` (handles division by zero)
- **Unsigned & Signed (Two's Complement) Modes**
- **Live Interactive Schematic**: SVG circuit diagram with animated active signal routing, probe indicators, and output LEDs
- **Flags**: Carry Out (`Cout`), Borrow Out, Overflow, Zero (`Z`), and Remainder
- **Reference & Original Diagram Tabs**: Includes the original schematic and opcode truth table

## Usage

Open `index.html` directly in any modern web browser.
