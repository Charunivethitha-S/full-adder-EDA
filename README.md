# full-adder-EDA
A Full Adder is implemented in Verilog with complete testbench and waveform simulation using EDA Playground, demonstrating fundamental digital logic design and verification skills.
# Full Adder in Verilog (EDA Playground)

This project implements a **Full Adder** using **Verilog HDL**, simulated on **EDA Playground**. It includes the RTL design, testbench, and waveform output for verification of all input combinations. This project demonstrates fundamental combinational logic design, simulation, and verification skills.

---

##  Project Contents
- **RTL Code** – Verilog implementation of the Full Adder  
- **Testbench** – Stimulus to verify Sum and Carry outputs  
- **Waveform (JPG/PNG)** – Simulation results to validate the design  
- **VCD Generation** – Using `$dumpfile` and `$dumpvars`  

---

##  Full Adder Overview
A Full Adder adds three 1-bit inputs (**A**, **B**, **Cin**) and produces two outputs:
- **Sum = A ⊕ B ⊕ Cin**
- **Carry = (A & B) | (B & Cin) | (A & Cin)**

Truth Table:

| A | B | Cin | Sum | Carry |
|---|---|-----|-----|-------|
| 0 | 0 |  0  |  0  |   0   |
| 0 | 0 |  1  |  1  |   0   |
| 0 | 1 |  0  |  1  |   0   |
| 0 | 1 |  1  |  0  |   1   |
| 1 | 0 |  0  |  1  |   0   |
| 1 | 0 |  1  |  0  |   1   |
| 1 | 1 |  0  |  0  |   1   |
| 1 | 1 |  1  |  1  |   1   |

---

##  Tools Used
- **EDA Playground** (Online Verilog Simulator)  
- **Verilog (IEEE 1364)**  
- **VCD waveform viewer**

**How to Run**

1.Open the RTL file (full_adder.v) and the testbench (full_adder_tb.v) in EDA Playground or any Verilog simulator (ModelSim, Icarus Verilog, etc.).

2.Ensure the testbench includes the VCD commands to capture waveforms:

$dumpfile("dump.vcd");
$dumpvars(0, full_adder_test_bench);


3.Run the simulation.

4.Open the generated dump.vcd file in a waveform viewer (e.g., EPWave) to observe the signal transitions.

**Outputs**

All possible input combinations (A, B, Cin) are applied.

Sum and Carry outputs matches the truth table

The waveform image included in the repository visually confirms the correctness of the design and verifies signal transitions for all inputs
---

