# Audio Amplifier Design and Hardware Implementation

> A complete multi-stage audio amplifier designed, simulated in **LTspice**, mathematically analyzed and validated on hardware.

---

## Project Overview

This project presents the design and implementation of a **four-stage audio amplifier** capable of amplifying low-level microphone signals into a power level suitable for driving a loudspeaker.

Unlike a simulation-only project, every stage was

- Designed analytically
- Derived mathematically
- Simulated in LTspice
- Built on hardware
- Experimentally verified using an oscilloscope

---

## Final Architecture

```
Microphone
     │
     ▼
Microphone Bias Circuit
     │
     ▼
Differential Amplifier
(Pre-Amplifier)
     │
     ▼
Common Emitter
Voltage Amplifier
     │
     ▼
Active Band-Pass Filter
20 Hz – 20 kHz
     │
     ▼
Class-AB Power Amplifier
     │
     ▼
Speaker
```

---

# Project Highlights

- LTspice Simulation

- Hardware Implementation

- Mathematical Derivations

- Frequency Response Analysis

- Oscilloscope Validation

- Total Harmonic Distortion Analysis

- Slew Rate Measurement

- CMRR Analysis

---

# Design Stages

## 1. Microphone Input Circuit

Provides DC biasing for the condenser microphone while coupling the AC audio signal into the amplifier chain.

Topics covered:

- Condenser microphone operation
- Bias resistor selection
- Coupling capacitor design

---

## 2. Differential Amplifier (Pre-Amplifier)

Designed using a matched BJT differential pair to amplify weak microphone signals while rejecting common-mode noise.

Analysis includes

- DC Bias Analysis
- Small Signal Model
- Gain Derivation
- Component Design
- Input Impedance
- Output Impedance
- CMRR Derivation
- LTspice Validation
- Hardware Verification

---

## 3. Common Emitter Gain Stage

Provides the majority of the voltage gain.

Includes

- Voltage Divider Bias Design
- Active Region Verification
- Maximum Output Swing
- Gain Derivation
- Small Signal Analysis
- Hardware Validation

---

## 4. Active Band-Pass Filter

Filters unwanted frequency components while preserving the audible frequency band.

Specifications

- Passband:
  - **20 Hz – 20 kHz**

Includes

- Transfer Function
- Frequency Response
- Cutoff Frequency Design
- Bode Analysis

---

## 5. Class-AB Power Amplifier

Final output stage used to deliver sufficient current to the speaker.

Includes

- Push-Pull Configuration
- Biasing Design
- Efficiency Analysis
- Output Power Calculation
- Unity Voltage Gain Verification

---

# Performance Analysis

The complete amplifier was evaluated using

- Transient Analysis
- AC Sweep
- Frequency Response
- Bode Plot
- Total Harmonic Distortion
- Slew Rate
- Hardware Measurements

---

# Performance Summary

| Parameter | Value |
|-----------|---------:|
| Overall Gain (10 mV Input) | **508.9** |
| Overall Gain (20 mV Input) | **449.5** |
| CMRR | **30.4 dB** |
| Slew Rate | **0.057 V/μs** |
| THD (10 mV Input) | **3.89%** |
| THD (20 mV Input) | **11.86%** |
| Stability Factor | **11.10** |

---

# Hardware Validation

The amplifier was physically implemented on a breadboard and experimentally validated using

- Oscilloscope
- Function Generator
- Condenser Microphone
- Dual Power Supply

Measured hardware results closely matched LTspice simulations.

---

# Repository Structure

```
Audio-Amplifier/
│
├── README.md
│
├── LTspice/
│   ├── Differential Amplifier.asc
│   ├── CE Amplifier.asc
│   ├── BandPass Filter.asc
│   ├── ClassAB Amplifier.asc
│   └── Complete Amplifier.asc
│
├── Reports/
│   ├── Audio Amplifier Design Report.pdf
│   ├── Full Circuit Analysis.pdf
│   └── Individual Component Analysis.pdf
│
└── Images/
    ├── Hardware/
    ├── Schematics/
    ├── Waveforms/
    └── BodePlots/
```

---

# Software Used

- LTspice
- Analog Electronics
- BJT Circuit Design
- Oscilloscope
- Function Generator

---

# Documentation

The repository contains

- Complete design report
- Mathematical derivations
- LTspice schematics
- Simulation results
- Hardware implementation
- Oscilloscope outputs
- Performance evaluation

---

# Future Improvements

- PCB Design
- Reduced THD
- Higher Output Power
- Thermal Compensation
- Closed-Loop Feedback
- Improved Power Efficiency

---

## Authors

**Yogesh Krishna**  
IIIT Hyderabad

**Anumay Rai**  
IIIT Hyderabad
