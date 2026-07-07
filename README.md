# FPGA VGA Game

## 📌 Project Overview

This project is a VGA-based arcade game implemented using **Verilog HDL** on an FPGA platform.

The game was developed as part of a digital circuit design course to gain practical experience in RTL design, finite state machine (FSM) implementation, VGA display control, keyboard input processing, collision detection, and hardware debugging.

---

## 👨‍💻 My Role

- Designed and verified FSM-based game logic
- Implemented RTL for game state control
- Analyzed Waveforms to identify state transition issues
- Redesigned the state register and Next-State Logic
- Created Testbench for repeated verification
- Verified operation on FPGA hardware

---

## 🛠️ Skills

- Verilog HDL
- FPGA
- RTL Design
- FSM (Finite State Machine)
- VGA Controller
- PS/2 Keyboard
- ModelSim
- Quartus Prime

---

## 🎮 Main Features

- VGA display output
- FSM-based game flow
- PS/2 keyboard control
- Random obstacle generation using LFSR
- Collision detection
- Multi-stage game progression

---

## 🔍 Problem Solving

During development, multiple game states shared the same coordinate register, causing previous position data to remain after state transitions.

I analyzed the waveform and found that the input paths inside the Next-State Logic were not properly separated.

To solve this problem, I redesigned the FSM by separating the State Register and Next-State Logic and assigned independent registers for each game mode.

After the redesign, I verified the behavior through simulation using Testbench and confirmed the operation on the FPGA board.

---

## 📚 What I Learned

This project helped me understand how to analyze digital systems rather than simply modifying code.

Through waveform debugging, RTL verification, and FSM redesign, I learned how hardware architecture directly affects system stability and performance.

---

## ⚠️ Project Preservation Note

This repository contains the remaining source code from an undergraduate FPGA project.

Because the project was completed several years ago, some source files and the original development environment were no longer available.

The repository has been organized using the remaining source code and project documentation.
