# Stick Hero Application



Welcome to the Stick Hero Application! This is a simple JavaFX game where the player controls a character by extending a stick to cross platforms. The goal is to reach the next platform without falling.

## Index

- [Features](#features)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Run the Application](#run-the-application)
  - [Game Controls](#game-controls)
- [Structure of the Project](#structure-of-the-project)
  - [Packages and Classes](#packages-and-classes)
  - [Resources](#resources)
- [How to Play](#how-to-play)
- [Additional Notes](#additional-notes)
- [First Iteration](#first-iteration)
- [Final Version](#final-version)
- [Game Demo](#game-demo)
- [Class Explanations](#class-explanations)
  - [Controller Class](#controller-class)
    - [Game State and Parameters](#game-state-and-parameters)
  - [Pillars Class](#pillars-class)

## Features

- **Gameplay**: Extend the stick by clicking and holding the mouse, and release to drop the stick.
- **Scoring**: Score points for successfully reaching the next platform.
- **Sound Effects**: Enjoy sound effects for various actions in the game.
- **Exit Confirmation**: A confirmation dialog is provided when attempting to exit the game.

## Getting Started

### Prerequisites

- Ensure you have Java installed on your machine.

### Run the Application

- Execute the `StickHeroApplication` class to start the game.

### Game Controls

- Click and hold the mouse to extend the stick.
- Release the mouse to drop the stick and move the character.

## Structure of the Project

### Packages and Classes

- `com.example.stickheroapplication`: Main package containing the application code.
  - **StickHeroApplication**: Main class to launch the application.
  - **Controller**: Controller class for the gameplay screen.
  - **Diamond**: Class representing a collectible diamond in the game.
  - **Pillars**: Class handling the generation of platforms in the game.
  - **SaveGame**: Class representing a saved game state.
  - **SceneController**: Controller class for the home screen.

### Resources

- **images**: Folder containing image resources used in the application.

## How to Play

1. Launch the game.
2. Click and hold the mouse to extend the stick.
3. Release the mouse to drop the stick and move the character.
4. Reach the next platform to score points.

## Additional Notes

- This project uses JavaFX for the graphical user interface.
- Sound effects are incorporated to enhance the gaming experience.
- The game features a confirmation dialog when attempting to exit.

## First Iteration

The first iteration of the Stick Hero Application focused on establishing the core gameplay mechanics. This version included the basic functionality of extending a stick to reach the next platform. The initial release was designed to test the fundamental concept and gather feedback for future enhancements.

| **Start**      | **Retry**        |
|---------------------|---------------------|
| ![Start Page](/Images/start.png) | ![End Page](/Images/end.png) |

| **Character**       | **Stick Increase**  |
|---------------------|---------------------|
| ![Character](/Images/chr.png) | ![Stick Increase](/Images/stick.png) |

#### Key Features of the First Iteration:

- **Basic Stick Extension Mechanism**: Players could click and hold the mouse button to extend the stick and release it to let the character walk across.
- **Simple Scoring System**: Points were awarded based on the accuracy of the stick length in relation to the next platform.
- **Minimalist Graphics**: The game featured simple graphics to keep the focus on the gameplay.
- **Feedback Collection**: An option was provided for players to submit feedback directly through the game interface.

This iteration laid the groundwork for subsequent updates, which introduced additional features such as sound effects, scoring enhancements, and improved graphics.

## Final Version

| **Start**      | **Game Over**        |
|---------------------|---------------------|
| ![Start Page](/Images/fstart.png) | ![End Page](/Images/gameover.png) |

| **Character**       | **Stick Increase**  |
|---------------------|---------------------|
| ![Character](/Images/fchr.png) | ![Stick Increase](/Images/fstick.png) |

## Game Demo

<p align="center">
  <img src="/Images/demo.gif" alt="Game Demo">
</p>

## Class Explanations

### Controller Class

The `Controller` class is a crucial component in the Stick Hero Application. It serves as the controller for the gameplay screen, managing the game logic, user interactions, and transitions between different game states. Key aspects of the `Controller` class include:

- **gameScreen**: A `Pane` representing the main game screen where platforms and characters are displayed.
- **score**: A `Label` displaying the current score of the player.
- **stickHero**: An `ImageView` representing the character in the game.

#### Game State and Parameters

- **endGame()**: Method to handle the end of the game, triggering the character's fall and displaying the game over message.
- **displayGameOverMessage()**: Method to display the game over message with a fade transition.
- **switchToMainScreen()**: Method to transition to the main screen after the game is over.

### Pillars Class

The `Pillars` class in the Stick Hero Application is responsible for generating and handling the properties of the platforms (pillars) in the game. Key aspects of the `Pillars` class include:

- **Extends Rectangle**: The `Pillars` class extends the `Rectangle` class, indicating that it inherits properties and methods from `Rectangle`. This allows `Pillars` to be visually represented as rectangles.
- **random**: An instance of the `Random` class for generating random values.
- **screenWidth**: The width of the game screen.
- **PLATFORM_HEIGHT**: The constant height of the platforms.
- **minWidth** and **maxWidth**: The minimum and maximum width of the platforms.
- **layoutY**: The y-coordinate at which the platforms are placed.
- **minLayoutX** and **maxLayoutX**: The minimum and maximum x-coordinates for placing the platforms.

---

Enjoy playing Stick Hero! If you encounter any issues or have any questions, feel free to reach out for support. Happy gaming!
