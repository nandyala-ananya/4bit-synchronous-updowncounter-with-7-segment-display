4-Bit Synchronous Up/Down Counter with 7 segment Display (NI Multisim)

Overview

This project implements a 4-bit synchronous up/down counter designed and simulated using NI Multisim.
The counter counts either up or down based on a control input and displays the current count on a HEX seven-segment display.

The circuit is built using JK flip-flops and basic logic gates, demonstrating the working of synchronous counters and digital logic design.

Features

- 4-bit synchronous counting
- Supports both Up and Down counting modes
- Implemented using JK Flip-Flops (7476 IC)
- Uses logic gates (7408 AND, 7432 OR, 7404 NOT) for control logic
- Output displayed using HEX seven-segment display
- Designed and simulated in NI Multisim

Components Used

- 7476 – JK Flip-Flop IC
- 7408 – AND Gate IC
- 7432 – OR Gate IC
- 7404 – NOT Gate IC
- HEX Seven-Segment Display
- Clock Source (2 Hz, 5V)
- Switch for Up/Down control
- 5V Power Supply

Working Principle

The circuit consists of four JK flip-flops connected in synchronous mode, meaning all flip-flops share the same clock signal.

Logic gates are used to control the J and K inputs of each flip-flop depending on the current state and the Up/Down control signal.

- When the control input selects Up mode, the counter increments sequentially:
  
  "0000 → 0001 → 0010 → ... → 1111"

- When the control input selects Down mode, the counter decrements:
  
  "1111 → 1110 → 1101 → ... → 0000"

The 4-bit output (Q0–Q3) is connected directly to the HEX seven-segment display, which converts the binary output into the corresponding hexadecimal digit (0–F).

Simulation

The circuit is simulated in NI Multisim with a 2 Hz clock signal, allowing the counter output to change slowly so that the counting sequence can be clearly observed on the display.

Applications

- Digital counters
- Frequency division circuits
- Digital clocks and timers
- Sequential logic system design

Tools Used

- NI Multisim
- Digital Logic ICs (74xx series)

Author

Created as a Digital Electronics project to demonstrate the design and simulation of synchronous counters using logic gates and flip-flops.
