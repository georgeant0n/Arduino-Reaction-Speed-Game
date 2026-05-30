# Arduino Reaction Speed Game 🚦⏱️

A fun, fast-paced 2-player reaction speed game built with an Arduino Uno, LEDs, push buttons, and a buzzer. Test your reflexes and see who is the fastest!

## 🎮 How to Play

1. **The Countdown:** When the game starts, a sequence of lights acts like a traffic light (Green ➔ Yellow ➔ Red). Each light is accompanied by a short beep from the buzzer.
2. **The Anticipation:** Once the Red light turns on, you must wait. It will turn off after a **random** amount of time (between 0.9 to 4.9 seconds). 
3. **The Race:** The moment the Red light turns off, two White LEDs (one for each player) turn on simultaneously. 
4. **The Winner:** The first player to press their button wins the round! The winner's White LED will remain lit, the loser's LED will turn off, and a victory sound will play from the buzzer. 
5. **Restart:** The game automatically resets after a short delay for the next round.

## 🛠️ Components Used

* 1x Arduino Uno
* 1x Breadboard
* 2x Push Buttons (Player 1 & Player 2)
* 5x LEDs (1x Green, 1x Yellow, 1x Red, 2x White)
* 5x Resistors (for the LEDs)
* 1x Piezo Buzzer
* Jumper Wires

## 🔌 Pin Mapping

Based on the provided code and wiring diagram, here is the hardware setup:

| Component | Arduino Pin | Type |
| :--- | :---: | :--- |
| **Player 1 Button (Left)** | `13` | Input (Internal Pull-up) |
| **Player 1 LED (White)** | `12` | Output |
| **Green LED** | `11` | Output |
| **Yellow LED** | `10` | Output |
| **Red LED** | `9` | Output |
| **Player 2 LED (White)** | `8` | Output |
| **Buzzer** | `7` | Output |
| **Player 2 Button (Right)**| `6` | Input (Internal Pull-up) |

*Note: The `randomSeed()` is initialized using an unconnected analog pin (`A0`) to generate truly random delays for the red light.*

## 📸 Circuit Diagram

<img width="1333" height="1073" alt="image" src="https://github.com/user-attachments/assets/5dc05ed5-62da-4c63-80e8-7f23ebc275ad" />


## 🚀 How to Run

1. Clone or download this repository.
2. Open the `.ino` file in the **Arduino IDE**.
3. Connect your Arduino Uno to your computer via USB.
4. Select the correct Board and Port from the `Tools` menu.
5. Click **Upload** to flash the code to your Arduino.
6. Get a friend and start playing!
