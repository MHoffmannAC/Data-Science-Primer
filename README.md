# Hangman Game (Created during the WBS DataScience Primer)

## Project Overview

This Python project implements an advanced version of the classic Hangman game, featuring a user-friendly console interface, customizable settings, and support for multiple languages.

-----

### Settings:
<pre>
██   ██  █████  ███    ██  ██████  ███    ███  █████  ███    ██ 
██   ██ ██   ██ ████   ██ ██       ████  ████ ██   ██ ████   ██ 
███████ ███████ ██ ██  ██ ██   ███ ██ ████ ██ ███████ ██ ██  ██ 
██   ██ ██   ██ ██  ██ ██ ██    ██ ██  ██  ██ ██   ██ ██  ██ ██ 
██   ██ ██   ██ ██   ████  ██████  ██      ██ ██   ██ ██   ████

Available difficulties:
1:    Words - easy   (handpicked)
2:    Words - medium (random nouns)
3:    Words - hard   (random words)
4:    Sentence - hard (often gibberish)
5:    Use user input as solution
1984: Doublethink sentences

Available languages:
en: english
de: deutsch

Available illustrations:
hangman: Classical hangman figure
flowers: Field of flowers
chase:   Police chase

Enter difficulty to start a new game
or choose different language or illustration
</pre>

### Game screen:
<pre>                                        
_ R E E _ _ _   I S   S _ A _ E R _               wWWWw
                                                  (___) wWWWw                vVVVv
Available letters:                                 ~Y~  (___)                (___)
    C D   F G H                                    \|    ~Y~            |     ~Y~
J K L M N O   Q                               |   \ |/   \| /           |    \ |/
  T U V   X Y Z                             \\|// \\|// \\|/// \\|//  \\|// \\\|///
                                           ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
You have 3 wrong guesses left
</pre>
-----

## Features

- **Multi-Language Support**: The game supports both English and German, with the ability to easily add additional languages. Each language has custom messages and labels, ensuring a smooth user experience.

- **Difficulty Levels**: Players can choose from various difficulty levels, including:
  - Handpicked words.
  - Random nouns.
  - Random words or sentences.
  - Custom user input.
  - Sentences from Orwell's *1984*, adding a unique thematic challenge.

- **Multiple Illustrations**: The game includes different visual representations for the hangman, such as:
  - Classic Hangman Figure.
  - A field of flowers.
  - A police chase scene.

- **Sentence Support**: Unlike traditional Hangman, this version supports entire sentences as solutions, making it more challenging and interesting.

- **Custom Fonts and Visuals**: `PyFiglet` is used to enhance the visual presentation with stylized text headers, providing a more engaging console experience.

-----

## Coding Techniques

- **Function Abstraction**: Key gameplay elements like word selection, guess evaluation, and screen display are encapsulated in distinct functions. This abstraction separates concerns and makes the codebase easier to manage and debug.

- **Data-Driven Logic**: The game utilizes dictionaries to store language-specific settings, difficulty levels, and visual styles. This data-driven approach enables easy customization and scalability, allowing new languages, difficulties, or themes to be added with minimal code changes.

- **Input Validation and Error Handling**: The game includes robust input validation to ensure players provide valid guesses. It also handles errors gracefully, guiding users to correct their inputs without disrupting gameplay.

- **State Management and Update Mechanism**: The game tracks and updates the state of the game board, guessed letters, and remaining guesses efficiently. This is done through careful state management, ensuring that the game board accurately reflects the current progress and status.

- **Use of External Libraries**: Libraries like `wonderwords` and `pyfiglet` are leveraged to enhance functionality and user experience. `wonderwords` provides a dynamic word and sentence generation, while `pyfiglet` adds visual flair with stylized text headers.

- **Iterative Screen Updates**: The game uses console-clearing techniques to create a seamless and interactive experience. By refreshing the screen with updated game states after each guess, the game mimics the feel of a GUI in a console environment.


-----

## Project Files

- **Hangman_by_MHoffmann.ipynb**: The main Python script created using Google Colab and containing the full implementation of the game.
- **doppeldenk** and **doublethink**: Files containing sentences (in German and English, respectively) following the doublethink idea of Orwell's book 1984.
- **README.md**: This file, providing an overview of the project and instructions for use.

-----

## How to Play

1. **Start the Game**:
   - Run the script online using Google Colab or locally as a Jupyter notebook. The game will welcome you with a stylized header.

2. **Choose Settings**:
   - Select the difficulty level or change the language and visual style. 

3. **Play the Game**:
   - Guess letters or attempt to solve the entire word/sentence. The game will update the board and track your remaining guesses.

4. **End or Restart**:
   - Once the game ends, choose to restart or quit. The result screen will display whether you won or lost, along with the correct solution.

-----

## Installation and Setup

All necessary `pip install` calls are included in the notebook file. No additional setup is required. 
