# Snake 2.O Game Project
#### Video Demo: https://youtu.be/j4e5GvHzVyI

### HOW TO PLAY THE GAME:
Extract all files and double click the "Run_Game" windows batch file.

#### Description:
The Snake 2.O project is an enhanced version of the classic Snake game, built using Lua and the LÖVE framework. This iteration of the game offers a dynamic gaming experience where players guide a snake on a grid-like map, with the objective of expanding in length by devouring "food" items represented by vibrant green tiles. As the snake grows, the game's intensity escalates, providing players with an escalating level of challenge.

One standout feature is the inclusion of a "Rage Mode" that activates at specific intervals. In this mode, the game becomes even more demanding. All or some of the enemies freeze in their current positions, while the player's snake undergoes a dramatic increase in speed for a set duration. This intensification adds an extra layer of excitement and difficulty to the game.

Additionally, every fourth time a food item is consumed, a new enemy is introduced onto the map. This injection of new challenges keeps the gameplay fresh and engaging, requiring players to adapt to evolving circumstances.

To add a strategic element, players must be cautious to avoid turning all tiles on the map grey. This signifies excessive exploration and leads to a game over. This strategic aspect challenges players to navigate the map efficiently, minimizing tile exploration for a successful outcome.

### File Breakdown:

#### main.lua

The `main.lua` file serves as the entry point for the game. It orchestrates critical game components, such as initializing the tilemap, loading images, and managing game states. This file establishes the visibility flag for the start page (`startPageVisible`) and orchestrates transitions between the start screen, main game screen, and game over screen.

#### snake.lua

In `snake.lua`, the Snake class is defined. This class governs the behavior of the player-controlled snake. It handles movement, input processing, and collision detection. When the snake collides with the green "food," it experiences growth in length, mirroring the iconic snake movement mechanic.

#### enemy.lua

The `enemy.lua` file introduces the Enemy class. This class represents an autonomous snake that moves independently on the map. The enemy snake introduces an additional layer of challenge, behaving distinctly from the player-controlled snake. It follows randomized movement patterns, adding unpredictability and complexity to the gameplay.

### Design Considerations:

The project adheres to an object-oriented design paradigm, making use of the Classic library for Lua. This approach enhances modularity and code reusability. The game state management system utilizes boolean flags (`startPageVisible`, `gameOver`) to determine which elements are displayed on-screen at any given moment.

Collision detection is a pivotal aspect of the game and is handled by the `checkcollision` function. This function assesses whether the snake's head collides with a tile on the map. Upon collision, the snake undergoes growth, and a new food item is generated.

The inclusion of Rage Mode, dynamic enemy spawning, and the strategic win condition adds depth to the gameplay, encouraging players to employ varying strategies for success.

### Future Enhancements:

- **Scoring System**: Implement a scoring mechanism to track player performance and progress.
- **Level Progression**: Incorporate multiple levels with increasing difficulty to offer a sense of achievement and progression.
- **Audio Integration**: Introduce sound effects and background music to heighten the overall gaming experience.

The Snake 2.O Game Project provides a robust foundation for further expansion and customization. Its clean, object-oriented structure permits easy modification and addition of new features. Players can relish a nostalgic gaming experience while also exploring opportunities for innovation within the codebase. Enjoy playing and coding!
