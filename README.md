# 🚦 Traffic Light Controller using Verilog HDL

## 📌 Overview

This project implements a Finite State Machine (FSM) based Traffic Light Controller using Verilog HDL. The controller cycles through Red, Green, and Yellow traffic signals based on predefined timing values.

---

## ✨ Features

- FSM Based RTL Design
- Verilog HDL
- Asynchronous Reset
- Behavioral Simulation using Vivado XSim
- Testbench Included

---

## 🛠 Tools Used

- Xilinx Vivado
- Verilog HDL
- XSim Simulator

---

## 📥 Inputs

| Signal | Description |
|--------|-------------|
| clk | System Clock |
| rst | Active High Reset |

---

## 📤 Outputs

| Signal | Description |
|--------|-------------|
| red | Red LED |
| yellow | Yellow LED |
| green | Green LED |

---

## 🔄 State Sequence

RED → GREEN → YELLOW → RED

---

## 📂 Project Structure

Traffic-Light-Controller-Verilog/
├── rtl/
│ └── traffic_light.v
├── tb/
│ └── tb_traffic_light.v
├── docs/
│ ├── block_diagram.png
│ ├── state_diagram.png
│ └── waveform.png
└── README.md

---

## 📷 Block Diagram

**                    +-------------------------+
                    |     Traffic Light FSM   |
                    |                         |
Clock ----------->  |                         |
Reset ----------->  |                         |
                    +-------------------------+
                         |      |        |
                         |      |        |
                         V      V        V
                      +-----+ +------+ +------+
                      | Red | |Yellow| |Green |
                      +-----+ +------+ +------+**

---

## 🔁 FSM Diagram

                +---------+
                |   RED   |
                +---------+
                     |
          Counter = 5|
                     V
                +---------+
                | GREEN   |
                +---------+
                     |
          Counter = 5|
                     V
                +---------+
                | YELLOW  |
                +---------+
                     |
          Counter = 2|
                     |
                     +------------+
                                  |
                                  V
                              +---------+
                              |   RED   |
                              +---------+

---

## 📈 Simulation Waveform

<img width="251" height="208" alt="Screenshot 2026-07-03 083928" src="https://github.com/user-attachments/assets/dc086dab-ea4c-411f-9d89-ecf5dd77b1d5" />

---

## 🚀 Applications

- Smart Traffic Control
- Road Junction Automation
- Smart City Infrastructure
- Educational RTL Design Project

---

## 👨‍💻 Author

Mrityunjay
