# Snake Game 🐍

A classic snake game built using Python's `Tkinter` library. Guide the snake to eat the food, grow longer, and avoid running into walls or itself. Compete with yourself to achieve the highest score!

## Features

- **Classic Snake Gameplay**: Use arrow keys to control the snake.
- **Score Tracking**: Keep track of your current score and highest score.
- **"Try Again" Button**: Restart the game after a game over.
- **Adjustable Speed**: Slower gameplay to improve control.

## Prerequisites

Make sure you have **Python 3.x** installed.

## Installation

1. Clone this repository or download the code.

   ```bash
   git clone https://github.com/your-username/snake-game.git
   cd snake-game

2. Set up a virtual environment (optional but recommended):

   ```bash
   python3 -m venv .venv
   source .venv/bin/activate
   
3. Install dependencies. (This game uses tkinter, which is included in standard Python distributions.)

## How to Play

1. **Start the Game**:
   - Run the game by executing the following command:

     ```bash
     python main.py
     ```

2. **Control the Snake**:
   - Use the arrow keys to move the snake:
     - **Up**: Move the snake up
     - **Down**: Move the snake down
     - **Left**: Move the snake left
     - **Right**: Move the snake right

3. **Objective**:
   - Guide the snake to eat the red food to grow and increase your score.
   - Avoid hitting the walls or the snake’s own body.

4. **Game Over**:
   - The game ends when the snake collides with a wall or itself.
   - A **“Game Over”** message will appear.
   - Click the **“Try Again”** button to restart the game and try to beat your highest score.


## Code Overview

### Main Components

- **Snake Class**: Manages the snake’s body and movements.
- **Food Class**: Generates random food positions on the canvas.
- **Game Logic**: Controls the game loop, score updates, collision detection, and restart functionality.

### Key Functions

- `next_turn(snake, food)`: Handles the snake’s movement and collision detection.
- `change_direction(new_direction)`: Changes the snake’s direction based on arrow key input.
- `check_collisions(snake)`: Checks for collisions with the walls and the snake’s body.
- `game_over()`: Displays “Game Over” text and shows the “Try Again” button.
- `restart_game()`: Resets the game state and starts a new game.

### Variables

- `SPEED`: Controls the game’s speed; adjust for faster or slower gameplay.
- `score` and `highest_score`: Track the current and highest scores.

## Customization

You can adjust game settings for a personalized experience:

- **Speed**: Change the `SPEED` variable for faster or slower gameplay.
- **Colors**: Modify `SNAKE_COLOR`, `FOOD_COLOR`, and `BACKGROUND_COLOR` for different visual styles.
- **Size**: Adjust `GAME_WIDTH`, `GAME_HEIGHT`, and `SPACE_SIZE` for different board sizes and snake lengths.
