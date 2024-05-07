# Minefield Game

This C++ program simulates a basic minefield game, similar to the classic Minesweeper. It employs simple console commands for user interaction. The game uses fixed field dimensions, with the current version set at 5 columns and 8 rows. As players progress in programming, they could update the game to accept dynamic field sizes.

## Features
- **Fixed Minefield Dimensions:** 5x8 grid to simplify the understanding and debugging process.
- **Modular Code Structure:** Functions are used to manage game logic, improving readability and maintainability.
- **Game States:** Game progress is tracked with flags and mine counts, changing states based on user actions.
- **Seed-based Randomization:** Ensures reproducibility of mine placement for testing by using a configurable seed.

## Game States
Cells in the game can be in one of several states:
1. **Unknown:** Cell has not been revealed.
2. **Unflagged Mine:** Cell contains a mine that hasn't been flagged.
3. **Flagged Mine:** Cell contains a mine and has been correctly flagged.
4. **Incorrectly Flagged Mine:** Cell does not contain a mine but has been flagged.

## Compilation/Execution
1. Ensure that your system has a C++ compiler installed.
2. Compile the code using the following command: ```g++ main.cpp -o minefield```
3. Run the program: ```./minefield```

## Gameplay
1. **Start the game:** The game initializes with a random placement of mines based on the seed.
2. **Commands:**
   - ```f X Y```: Flag the cell at coordinate (X, Y) as a mine.
   - ```r X Y```: Reveal the cell at coordinate (X, Y).
   - ```u X Y```: Unflag the cell at coordinate (X, Y).
3. **Winning the Game:** Avoid all mines and flag all correctly to win the game.

## Future Enhancements
- **Dynamic Field Sizes:** Allow users to specify the size of the minefield at the start.
- **Improved UI:** Implement a graphical user interface using libraries such as SFML or SDL.
- **Advanced Features:** Add features like saving the game state or multi-level difficulty.

## Contributing
Contributions to the project are welcome. Please ensure to follow the existing coding style and add comments where necessary. For major changes, please open an issue first to discuss what you would like to change.
