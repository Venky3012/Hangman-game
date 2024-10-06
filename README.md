# Hangman Game

This is a simple Python implementation of the classic "Hangman" word-guessing game. The game randomly selects a word from a predefined list, and the player must guess the word one letter at a time before running out of lives.

---

## How to Play

1. The game starts by displaying a logo and selecting a random word from the provided `word_list`.
2. The word is represented as underscores (`_`), each underscore representing a letter that needs to be guessed.
3. The player is prompted to input a single letter guess.
4. If the guessed letter is correct, it will replace the corresponding underscores in the word.
5. If the guessed letter is incorrect, the player loses one of the 6 lives.
6. The player continues guessing letters until either:
   - All letters are correctly guessed (the player wins), or
   - The player runs out of lives (the player loses).
7. The player will be notified after each guess whether they’ve won or lost a life.

---

## Project Files

- **`hangman.py`** - The main script that runs the game logic.
- **`hangman_words.py`** - This file contains the `word_list` variable, a list of potential words the game will randomly choose from.
- **`hangman_art.py`** - This file contains:
  - `stages` variable, which holds ASCII art representations of the hangman for each life stage.
  - `logo` variable, which holds the game logo as ASCII art.

---

## Game Rules

- The player is allowed 6 incorrect guesses (represented by 6 lives).
- The game ends when:
  - The player guesses all letters correctly, or
  - The player runs out of lives.
- The player cannot guess the same letter more than once (repeated guesses will prompt a message but won’t affect lives).

---

## Example Game Flow

### Initial Display:
