# DSC Snake Game Tournament

## Overview
This is a simple two-player Snake game developed for the DSC W25 BOT Event. The game is built using **HTML, and CSS.**

## Features
- **Two-player gameplay**: Player 1 controls a green snake, and Player 2 controls a blue snake.
- **Grid-based movement**: Players navigate using `WASD` (Player 1) and arrow keys (Player 2).
- **Food collection**: Snakes grow when they eat food.
- **Collision mechanics**:
  - Snakes freeze temporarily upon self or opponent collision.
  - Snakes freeze for 2 seconds if they hit the border.
- **Game timer**: 3-minute countdown to determine the winner.
- **Score tracking**: Scores update dynamically as players eat food.

## How to Play
2. **Player controls**:
   - **Player 1 (Green Snake)**: Move with `W` (up), `A` (left), `S` (down), `D`.
   - **Player 2 (Blue Snake)**: Move with arrow keys.
3. **Objective**:
   - Eat food to grow your snake.
   - Avoid hitting yourself, the opponent, or the game borders.
   - The player with the highest score at the end of 3 minutes wins.
4. **Game Over**:
   - When the timer reaches 0, the game displays final scores.
   - Click "Back" to return to the home screen.

## Technical Details
- **Canvas-based rendering**: The game uses an HTML `<canvas>` element for graphics.
- **JavaScript game loop**: Runs at 10 frames per second (`setInterval` function).
- **Snake behavior**:
  - Movement is grid-based (20px per step).
  - Directional changes are handled in the `handleKeyPress` function.
  - Freezing mechanics prevent movement for a short duration after collisions.
- **Food generation**: Randomly placed within the canvas boundaries.
- **Score updates**: Displayed in real-time in the game UI.

## Future Improvements
- Add sound effects for eating food and collisions.
- Enhance graphics with animations and smoother transitions.

## Running the Game
Open the `index.html` file in a browser to play.
