# FPGA VGA Game

FPGA 기반 VGA 게임 프로젝트입니다.

Verilog HDL을 사용하여 VGA 출력, FSM(Finite State Machine), PS/2 키보드 입력, LFSR 기반 랜덤 생성 및 충돌 판정을 구현했습니다.

---

## 📌 Project Overview

This project is a VGA-based arcade game implemented using Verilog HDL on an FPGA platform.

The project was developed during a digital circuit design course to practice RTL design, FSM implementation, VGA display control, keyboard input processing, collision detection, and hardware debugging.

---

## 👨‍💻 My Role

- Designed FSM-based game logic
- Implemented RTL for game state control
- Analyzed Waveforms to identify state transition issues
- Redesigned the State Register and Next-State Logic
- Developed Testbench for repeated verification
- Verified functionality on FPGA hardware

---

## 🛠️ Skills

- Verilog HDL
- FPGA
- RTL Design
- FSM
- VGA Controller
- PS/2 Keyboard
- ModelSim
- Quartus Prime

---

## 🎮 Main Features

- VGA display output
- FSM-based game flow
- PS/2 keyboard control
- LFSR-based random obstacle generation
- Bounding box collision detection
- Multi-stage game progression

---

## 🔍 Problem Solving

During development, multiple game states shared the same coordinate register, causing previous position data to remain after state transitions.

By analyzing simulation waveforms, I found that the input paths inside the Next-State Logic were not properly separated.

To solve the issue, I redesigned the FSM by separating the State Register and Next-State Logic, and assigned independent registers for each game state.

The redesigned logic was verified through Testbench simulation and FPGA hardware testing.

---

## 📚 What I Learned

Through this project, I learned how to analyze digital systems by tracking signal flow and debugging waveforms rather than simply modifying code.

It also helped me better understand FSM design, RTL verification, and hardware-oriented problem solving.

---

## ⚠️ Project Preservation Note

This repository contains the remaining source code from an undergraduate FPGA project.

Some source files and the original development environment were not preserved after the project was completed. The repository has therefore been organized using the remaining source code and project documentation.
