# Hangman Game (Created during the WBS DataScience Primer)

## Project Overview

This Python project implements an advanced version of the classic Hangman game, featuring a user-friendly console interface, customizable settings, and support for multiple languages.

-----

## Features

- **Multi-Language Support**: The game supports both English and German, with the ability to easily add additional languages. Each language has custom messages and labels, ensuring a smooth user experience.

- **Difficulty Levels**: Players can choose from various difficulty levels:
  - **Easy**: Handpicked words.
  - **Medium**: Random nouns.
  - **Hard**: Random words or sentences.
  - **Custom**: Users can input their own solution.
  - **1984 Mode**: Uses sentences from Orwell's *1984*, adding a unique thematic challenge.

- **Multiple Illustrations**: The game includes different visual representations for the hangman, such as:
  - Classic Hangman Figure.
  - A field of flowers.
  - A police chase scene.

- **Sentence Support**: Unlike traditional Hangman, this version supports entire sentences as solutions, making it more challenging and interesting.

- **Custom Fonts and Visuals**: PyFiglet is used to enhance the visual presentation with stylized text headers, providing a more engaging console experience.

-----

## Coding Techniques

- **Modular Design**: The game is organized into modular functions, each responsible for a specific task, such as evaluating guesses, displaying the game screen, and managing the game state. This modular approach makes the code easier to read, maintain, and extend.

- **Flexible Input Handling**: The game can handle both single-letter inputs and full-word or sentence guesses, adding versatility to how players interact with the game. It also includes input validation to ensure that only valid guesses are processed.

- **Randomized Content Generation**: The game uses external libraries like `wonderwords` and custom functions to generate random words and sentences, providing a fresh experience with each playthrough. This feature also allows for themed content, like sentences from *1984*, to be easily integrated.

- **Dynamic Difficulty Adjustment**: The game supports multiple difficulty levels by dynamically selecting content generation functions based on the player’s choice. This technique allows the game to adapt to the player’s skill level.

- **Enhanced User Feedback**: The game provides real-time feedback on guesses, updating the visual representation of the hangman and available letters. This immediate response helps to keep the player engaged and informed about their progress.

- **Localization Support**: The game is designed to easily support multiple languages. All user-facing messages are stored in a dictionary, allowing for quick translation and adaptation to different languages without altering the core game logic.

-----

## Project Files

- **Hangman_by_MHoffmann.ipynb**: The main Python script created using Google Colab and containing the full implementation of the game.
- **doppeldenk** and **doublethink**: Files containing sentenced (in German and English, respectively) following the doublethink schema of Orwell's book 1984.
- **README.md**: This file, providing an overview of the project and instructions for use.

-----

## How to Play

1. **Start the Game**:
   - Run the script in Google Colab. The game will welcome you with a stylized header.

2. **Choose Settings**:
   - Select the difficulty level, language, and visual style. 

3. **Play the Game**:
   - Guess letters or attempt to solve the entire word/sentence. The game will update the board and track your remaining guesses.

4. **End or Restart**:
   - Once the game ends, choose to restart or quit. The result screen will display whether you won or lost, along with the correct solution.

-----

## Installation and Setup

No additional setup is required. The necessary pip install calls are included in the Colab file.
