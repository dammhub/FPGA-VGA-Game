# FPGA VGA Game Architecture

## Overall Structure

```
               CLOCK
                 │
        Clock Generator
                 │
        VGA Timing Controller
                 │
     ┌───────────┴───────────┐
     │                       │
PS/2 Keyboard           Game FSM
                             │
        ┌────────────────────┼────────────────────┐
        │                    │                    │
 Random Generator      Object Controller   Collision Detection
        │                    │                    │
        └────────────────────┴────────────────────┘
                             │
                       RGB Generator
                             │
                        VGA Display
```

---

## Main Modules

### GAME

Top module responsible for integrating the entire game system.

### VGA Timing Controller

Generates horizontal and vertical counters for VGA output.

### Game FSM

Controls the overall game state.

- Start
- Stage 1
- Stage 2
- Stage 3
- Game Clear
- Game Over

### Random Generator

Uses a 16-bit LFSR to generate pseudo-random values for obstacle speed.

### Collision Detection

Checks whether the player collides with obstacles using bounding box collision.

### Keyboard Interface

Receives PS/2 keyboard input and updates player movement.

---

## My Contribution

- FSM implementation
- RTL design
- Waveform debugging
- Next-State Logic redesign
- Testbench verification
- FPGA board verification
