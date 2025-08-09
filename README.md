# PIC LED Catch Game 🎮💡

**Built on Proteus Simulation Software**

---

## 🎯 Project Overview

This project is a simple **PIC-based LED Catch Game** designed and simulated using **Proteus**. The game randomly lights up one LED at a time, and the player’s goal is to **“catch” the lit LED** by pressing the corresponding button. Every successful catch increments the player’s score, which is displayed on two seven-segment displays.

---

## 🔍 Initial Idea and Introduction

- LEDs light up **randomly one at a time**.  
- Player presses the button corresponding to the lit LED to score a **“catch.”**  
- The score is displayed on **two 7-segment displays**, showing values from 0 to 99.  

---

## 🛠️ Equipment & Components Used

- **Clocks** (two clocks at 250 ms and 500 ms frequencies)  
- **Logic Gates:** NOT Gate, AND Gate, OR Gate  
- **LEDs** (4 LEDs for the game interface)  
- **Resistors** (including 10K pull-up resistors for buttons)  
- **Buttons** (4 input buttons, one for each LED)  
- **Ground and 5V Vcc Power Supply**  
- **4-bit Binary Ripple Counters (74LS93)** for score counting  
- **4-bit Comparator** to compare button presses with LEDs  
- **Seven Segment Displays** (2 units for displaying score 0-99)  
- **Wires and Connections** as per circuit design  

---

## ⚙️ Procedure & Working

1. Two clocks run at different frequencies — **250 ms and 500 ms** — driving a **Demultiplexer (74LS138)** to randomly light up one of the four LEDs.  
2. Four buttons are connected, each linked to ground on one side and a 10K resistor with 5V on the other to ensure proper input signals.  
3. Outputs from the LEDs and buttons are fed into a **4-bit comparator** which outputs a logical HIGH (`1`) **only if the pressed button matches the lit LED**.  
4. The comparator’s output triggers the first **4-bit binary ripple counter (74LS93)** which increments the score from 0 to 9.  
5. When the first counter overflows, a second 4-bit binary ripple counter increases the score range from 9 up to 99.  
6. Both counters output to **two seven-segment displays**, visually showing the player’s current score.  

---

## 🖥️ Simulation Details

- The entire circuit and logic were designed and tested on **Proteus Simulation Software**.  
- Proteus allowed real-time simulation of the clocks, gates, buttons, LEDs, counters, and seven-segment displays, accurately reflecting the game mechanics and scoring system.  

---

## 🎮 How to Play

- Watch for the LED that lights up randomly.  
- Press the button corresponding exactly to the lit LED.  
- Each correct press increments the score by one.  
- The game score is displayed on the two 7-segment displays, counting from 0 up to 99.  

---

## 📂 Project Files

- Proteus schematic files (.DSN)  
- Simulation configurations  
- Circuit diagrams and design notes  

*(Make sure you have Proteus installed to run and modify the simulation)*

---

## 📞 Contact

For questions, feedback, or collaboration:  
✉️ mabsarkhalid@gmail.com 
🔗 [LinkedIn Profile](www.linkedin.com/in/muhammad-absar-khalid-58aa18293)

---

Enjoy catching those LEDs and have fun with your Proteus simulation! 💡🎉
