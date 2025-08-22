# 🚀 Skydrome - FPGA Game

<p align="center">
  <img src="https://img.shields.io/badge/Verilog-F0DB4F?style=for-the-badge&logo=verilog&logoColor=white" />
  <img src="https://img.shields.io/badge/FPGA-DE2--115-008000?style=for-the-badge&logo=altera&logoColor=white" />
  <img src="https://img.shields.io/badge/UFABC-0055A4?style=for-the-badge&logoColor=white" />
  <img src="https://img.shields.io/badge/7--Segment%20Displays-FF5733?style=for-the-badge&logoColor=white" />
  <img src="https://img.shields.io/badge/LEDs-FF0000?style=for-the-badge&logoColor=white" />
</p>

---

## 🎮 About the Game
Skydrome is a **real-time reaction game** implemented in **Verilog** for the **DE2-115 FPGA** board.  
Players must **fire at incoming green LEDs** and **block red LEDs** before the time runs out. The game tracks **score**, **remaining blocks**, and shows a **countdown timer**.

- **Clock**: 50 MHz  
- **Buttons**: Start, Reset, Fire, Pause, Block  
- **Inputs**: RA switches (for configuration)  
- **Outputs**: LEDs (red & green), 7-segment displays (score, blocks, timer), Game Over LED  

---

## ⚙️ Parameters

| Parameter | Default | Description |
|-----------|---------|-------------|
| `ADDSCR` | 50 | Points added per successful hit |
| `SUBGASTOU` | 10 | Points subtracted for wasted green shots |
| `SUBATINGIDO` | 15 | Points subtracted for hitting red |
| `MAX_BLOCKS` | 16 | Maximum blocks available |
| `CRONO_MAX` | 59 | Countdown timer max value |

---

## 🕹️ Gameplay Features

- **Score System**: Points added or subtracted based on hits/misses  
- **Blocks**: Limited blocks to stop red LEDs, displayed on 7-segment  
- **Timer**: Countdown timer from `CRONO_MAX` seconds  
- **Fire Mechanism**: Green LEDs move left to represent shots  
- **Red LED Scroll**: Red LEDs scroll and toggle based on game state  
- **Pause Function**: Pause anytime using the pause button  
- **Game Over**: LED lights up when timer reaches zero  

---
