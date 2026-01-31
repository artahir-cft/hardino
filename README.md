# Hardino: Hardware Dino Game

Hardino is a physical, Arduino-based recreation of the iconic Chrome Dinosaur game. This project brings the endless runner experience to real hardware using LEDs and simple electronics, making it a fun and interactive way to learn about embedded systems, game logic, and Arduino programming.

## Features
- **Inspired by Chrome Dino:** Faithfully mimics the gameplay of the Chrome offline dinosaur game.
- **Obstacle LEDs:** Seven LEDs represent obstacles moving towards the player.
- **Jump Mechanic:** Control the dino's jump using serial input (press Enter in the Serial Monitor).
- **Collision Detection:** Lose the game if you fail to jump over an obstacle.
- **Game Over Animation:** Visual and audio feedback when the game ends.
- **Randomized Obstacles:** Obstacles appear at random intervals for replayability.

## Hardware Requirements
- Arduino Uno (or compatible board)
- 7 LEDs (for obstacles)
- 2 LEDs (for dino: up and down positions)
- 1 Buzzer (for game over sound)
- Resistors (appropriate values for LEDs and buzzer)
- Jumper wires
- Breadboard

## Pin Configuration
| Pin | Function           |
|-----|--------------------|
| 2-8 | Obstacle LEDs      |
| 9   | Dino Down LED      |
| 10  | Dino Up LED        |
| 13  | Buzzer             |

## How to Play
1. **Upload the Code:**
	- Open `main.ino` in the Arduino IDE.
	- Connect your Arduino board and upload the sketch.
2. **Connect Hardware:**
	- Wire the LEDs and buzzer according to the pin configuration above.
3. **Start the Game:**
	- Open the Serial Monitor (baud rate: 9600).
	- Press Enter to make the dino jump over obstacles.
	- Avoid collisions to keep playing. If you collide, the game will reset automatically.

## Code Overview
- **Obstacle Movement:** LEDs light up in sequence to simulate obstacles moving left to right.
- **Jump Logic:** The dino can jump (switching LEDs) for a short duration when Enter is pressed.
- **Collision Detection:** If the dino is down when an obstacle reaches it, the game ends.
- **Game Reset:** After a game over, the Arduino resets to start a new game.

## Customization
- Adjust obstacle speed by changing the timing in the code.
- Modify the number of obstacles or add new features (e.g., score display, more sounds).

## License
This project is open-source and free to use for educational and personal purposes.

---
Inspired by the Chrome Dinosaur game. Created with Arduino IDE.