# PRD: Snake Game

## 1. Objective
Create a single-file browser game inspired by the classic Snake arcade game. The game should be playable directly in a browser without external dependencies and should follow the same lightweight approach as the existing Memory Game project.

## 2. Product Summary
This project is a simple single-page Snake game built using HTML, CSS, and JavaScript. It will allow a player to control a snake, collect food, avoid collisions, and grow in length while tracking score and game-over states.

## 3. Problem Statement
Players enjoy short, engaging browser games that are easy to run and play without installation. A lightweight Snake game offers a familiar and fun arcade experience while demonstrating front-end interactivity in a minimal setup.

## 4. Goals
- Build a playable Snake game in a single HTML file
- Keep the game accessible and easy to understand
- Support keyboard controls for fast gameplay
- Provide score tracking and restart behavior
- Maintain a polished and responsive game layout

## 5. Non-Goals
- Multiplayer support
- Sound effects or advanced animations beyond the basic game loop
- Server-side logic or backend persistence
- Mobile touch gestures in the first version

## 6. Target Users
- Casual players who want quick arcade gameplay
- Beginner developers learning DOM manipulation and JavaScript logic
- Users who enjoy simple browser games without setup

## 7. User Stories
- As a player, I want to move the snake with keyboard controls so I can play the game easily.
- As a player, I want the snake to grow when it eats food so the game feels rewarding.
- As a player, I want the game to end when I hit a wall or my own body so the challenge is clear.
- As a player, I want to see my score update so I can track progress.
- As a user, I want a restart option so I can play again after losing.

## 8. Functional Requirements
### Core Gameplay
- A snake should move on a grid-based play area.
- The player should be able to control direction using arrow keys or WASD.
- Food should appear at random empty positions.
- Eating food should increase score and length.
- If the snake hits the border or itself, the game ends.

### Interface Requirements
- Display a title and game instructions.
- Show current score and best score.
- Include a start/restart button.
- Show a game-over message when the player loses.

### Technical Requirements
- Use a single HTML file with embedded CSS and JavaScript.
- Keep code readable and organized.
- Avoid external libraries or dependencies.

## 9. UX Requirements
- The board should be visually clear and centered on the page.
- Colors should provide good contrast for the snake, food, and background.
- The game should respond immediately to controls.
- A restart action should be obvious and easy to access.

## 10. Acceptance Criteria
1. The page loads and shows the Snake game board.
2. The snake moves when the player presses arrow keys or WASD.
3. Food appears at random valid positions.
4. The snake grows after eating food and the score increases.
5. The game ends when the snake collides with the wall or itself.
6. A restart option allows the user to play again.
7. Best score is retained between sessions if browser storage is supported.
8. The game works without external dependencies.

## 11. Suggested Implementation Approach
- Create a fixed-size board using CSS Grid.
- Represent the snake as an array of coordinate objects.
- Update the snake position in timed intervals.
- Generate a food item on an empty grid cell.
- Check collision boundaries and self-collision logic.
- Trigger the game-over state and allow restart.

## 12. Risks and Considerations
- Direction changes can create accidental reversals if not handled carefully.
- Reset logic must clear the board state cleanly before a new round.
- Timing and frame updates should stay consistent and responsive.

## 13. Definition of Done
The Snake game feature is complete when the game can be launched from a browser, the player can play and restart successfully, and all core gameplay requirements are met without errors.
