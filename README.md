# CMOS Priority Encoder – Technology Scaling Analysis

## Overview
This repository presents the design and power analysis of an 8-to-3 CMOS priority encoder implemented across multiple technology nodes (250nm, 180nm, 45nm, and 16nm). The objective is to study the impact of technology scaling on power consumption and signal behavior using LTspice simulations.

## Motivation
With aggressive CMOS scaling, power efficiency has become a critical design metric in VLSI systems. Priority encoders are widely used in interrupt controllers, ADCs, and digital systems where low power and correct priority resolution are essential.

## Design Details
- Circuit Type: 8-to-3 CMOS Priority Encoder
- Logic Style: Static CMOS
- Tool Used: LTspice
- Load Capacitance: 100 µF
- Outputs: A, B, C, and Valid (V)

## Technology Nodes Analyzed
| Technology Node | VDD | Average Power |
|----------------|-----|---------------|
| 250 nm | 2.5 V | 10.816 µW |
| 180 nm | 1.8 V | 7.529 µW |
| 45 nm  | 1.0 V | 4.0687 µW |
| 16 nm  | 0.7 V | 1.7141 µW |

## Key Observations
- Power consumption reduces significantly with technology scaling.
- Lower nodes show faster settling and reduced delay.
- Minor propagation delays appear in larger nodes due to higher capacitance.

## Repository Structure
- `LTspice_Files/` – Simulation files for each technology node
- `Waveforms/` – Output waveform screenshots
- `Schematics/` – CMOS circuit schematics
- `Report/` – Full project report (PDF)

## Future Work
- Delay and PDP analysis
- Layout-level implementation
- Comparison with alternative logic styles
- Extension to higher-bit encoders

## Author
**Smarajit Mishra**  
M.Tech – VLSI Design and Embedded Systems  
Odisha University of Technology and Research
