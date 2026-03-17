# Register File and ALU Implementation

Course: Computer Organization & Assembly Language  
Tool: Digital Simulator (H. Neemann)

## Components

### Register File
- Four 8-bit registers (R0–R3)
- Two read ports
- One write port
- Register selection via multiplexers and decoder

### ALU
Implements arithmetic and transfer operations based on control signals.

| S1 | S0 | Cin | Operation |
|----|----|-----|----------|
|0|0|0|A + B|
|0|0|1|A + B + 1|
|0|1|0|A + B̅|
|0|1|1|A − B|
|1|0|0|Transfer A|
|1|0|1|Increment A|
|1|1|0|Decrement A|
|1|1|1|Transfer A|

## Repository Structure
- circuits/ : Digital simulator circuit files
- screenshots/ : testing screenshots
