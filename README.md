# FPGA VGA Game

FPGA-based VGA game implemented in Verilog HDL.

This project was developed as part of an undergraduate Digital Circuit Design course. It implements a simple arcade-style game featuring VGA graphics, FSM-based game control, PS/2 keyboard input, collision detection, and LFSR-based random obstacle generation.

---

## 📌 Project Overview

The project focuses on implementing digital hardware using Verilog HDL, from RTL design to FPGA verification.

Key components include VGA display control, finite state machine (FSM) design, keyboard input processing, random obstacle generation, collision detection, and multi-stage game control.

---

## 👨‍💻 My Contributions

- Designed the overall FSM architecture
- Implemented RTL for game control logic
- Analyzed simulation waveforms to identify state transition issues
- Redesigned the State Register and Next-State Logic
- Developed testbenches for functional verification
- Verified the design through simulation and FPGA hardware testing

---

## 🛠️ Tech Stack

- Verilog HDL
- FPGA
- RTL Design
- Finite State Machine (FSM)
- VGA Controller
- PS/2 Keyboard Interface
- Quartus Prime
- ModelSim

---

## 🎮 Features

- VGA graphics output
- FSM-based game control
- PS/2 keyboard input
- LFSR-based random obstacle generation
- Bounding box collision detection
- Multi-stage gameplay

---

## 🔍 Problem Solving

During development, multiple game states unintentionally shared the same coordinate register, causing position data to remain after state transitions.

Waveform analysis showed that the data paths in the Next-State Logic were not properly separated.

To resolve the issue, I redesigned the FSM by separating the State Register from the Next-State Logic and assigning independent registers to each game state.

The updated design was verified through repeated ModelSim simulations and FPGA hardware testing.

---

## 📚 What I Learned

This project gave me hands-on experience in RTL design, FSM implementation, waveform analysis, and FPGA verification.

More importantly, I learned to identify design issues by tracing signal flow and verifying hardware behavior instead of relying on trial-and-error code changes.

---

## ⚠️ Project Preservation Note

This repository contains the remaining source code from an undergraduate FPGA project.

Some dependent modules and the original development environment were not preserved after the project was completed. The repository has been organized using the remaining source code and documentation.
