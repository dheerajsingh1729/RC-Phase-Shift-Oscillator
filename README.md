# RC-Phase-Shift-Oscillator

# RC Phase Shift Oscillator

This repository contains the KiCad design files for a 1 kHz RC Phase Shift Oscillator built using an operational amplifier. The circuit uses a three-section RC feedback network to generate a sinusoidal output waveform.

## Overview

An RC Phase Shift Oscillator produces oscillations by using a resistor-capacitor ladder network to create a total phase shift of 180 degrees. An inverting amplifier adds another 180 degrees, making the total loop phase shift 360 degrees. This satisfies the Barkhausen criterion for sustained oscillation.

The design is targeted for approximately 1 kHz.

## Circuit Principle

The oscillation frequency for a three-section RC phase shift oscillator is:

```text
f0 = 1 / (2πRC√6)
For this design:

R = 10 kΩ
C = 16 nF
Therefore:

f0 ≈ 1020 Hz ≈ 1 kHz
The minimum amplifier gain required for oscillation is approximately:

|Av| ≥ 29
Therefore, the feedback resistor is selected as:

Rf = 29R ≈ 290 kΩ
Components Used
Component	Value / Part	Quantity
Op-Amp	LM741	1
Resistor	10 kΩ	3
Capacitor	16 nF	3
Feedback Resistor	290 kΩ	1
Power Supply	±12 V DC	1
Repository Contents
RC-Phase-Shift-Oscillator/
├── Rc oscillator.kicad_pro
├── Rc oscillator.kicad_sch
├── Rc oscillator.kicad_pcb
├── Rc oscillator.kicad_prl
├── Rc oscillator-backups/
├── fp-info-cache
└── README.md
Features
1 kHz sine wave oscillator design
Three-section RC phase shift feedback network
Op-amp based inverting amplifier
PCB layout designed in KiCad
Suitable for analog electronics laboratory experiments
Tools Used
KiCad for schematic and PCB design
LM741 op-amp for oscillator implementation
Oscilloscope for waveform verification
Expected Output
The circuit is expected to generate a sinusoidal waveform of approximately 1 kHz when powered using a dual DC supply.

Output waveform: Sine wave
Expected frequency: ~1 kHz
Supply voltage: ±12 V DC
Applications
Audio-frequency signal generation
Analog electronics laboratory experiments
Op-amp oscillator demonstration
RC network frequency analysis
PCB design practice using KiCad
References
D. Roy Choudhury, Linear Circuit Analysis and Design
R. A. Gayakwad, Op-Amps and Linear Integrated Circuits
A. S. Sedra and K. C. Smith, Microelectronic Circuits
Author
Dheeraj Singh
Department of Electronics and Communication Engineering
Central University of Rajasthan
Email: 2022btece004@curaj.ac.in

