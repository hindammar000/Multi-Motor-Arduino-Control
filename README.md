# Incredible Bombul - Multi-Motor Arduino Control (Tinkercad Simulation)

An Arduino-based simulation project that controls **four DC motors** using **two L293D motor driver ICs**. The system was designed and tested in **Autodesk Tinkercad**, demonstrating synchronized motor control through a predefined sequence of forward, reverse, and turning movements.

---

## Preview



![Circuit](circuit.png)

---

## Components Used

- Arduino Uno R3
- 2 × L293D Motor Driver ICs
- 4 × DC Motors
- Breadboard
- Jumper Wires
- 5V Power Supply (Tinkercad)

---

## Pin Configuration

| Motor | Enable (EN) | IN1 | IN2 | Driver |
|-------|------------:|----:|----:|--------|
| Motor 1 | D5 | D2 | D3 | L293D #1 |
| Motor 2 | D6 | D4 | D7 | L293D #1 |
| Motor 3 | D10 | D8 | D9 | L293D #2 |
| Motor 4 | D11 | D12 | D13 | L293D #2 |

---

## Project Structure

```
.
├── code.ino
├── circuit.png
├── DC_MOTOR_L293D_SIMULATION.pdf
└── README.md
```

---

## Features

- Control of four DC motors using Arduino Uno
- Dual L293D motor driver configuration
- Fully simulated in Autodesk Tinkercad
- Automated multi-stage movement sequence
- Simple and easy-to-understand Arduino code

---

## Movement Sequence

The Arduino continuously repeats the following movement pattern:

| Phase | Action | Duration |
|-------|--------|---------:|
| 1 | All motors move forward | 30 s |
| 2 | All motors move backward | 60 s |
| 3 | Motor 1 stops while the remaining motors change direction | 5 s |
| 4 | Alternate motor directions for turning | 5 s |

After completing Phase 4, the sequence restarts automatically.

---

## Simulation

The circuit was designed and tested using **Autodesk Tinkercad**, allowing verification of both the wiring connections and the programmed motor behavior before implementation on physical hardware.

---

## Files

- `code.ino` — Arduino source code
- `circuit.png` — Circuit screenshot
- `DC_MOTOR_L293D_SIMULATION.pdf` — Wiring schematic
- `README.md` — Project documentation

---

## License

This project was developed for educational purposes.
