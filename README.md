# Hangman-game

README for Hangman Game
Hangman Game - Python Project
This is a simple Python implementation of the classic "Hangman" word-guessing game. The game randomly selects a word from a predefined list, and the player must guess the word one letter at a time before running out of lives.

How to Play:
The game starts by displaying a logo and selecting a random word from the provided word_list.
The word is represented as underscores (_), each underscore representing a letter that needs to be guessed.
The player is prompted to input a single letter guess.
If the guessed letter is correct, it will replace the corresponding underscores in the word.
If the guessed letter is incorrect, the player loses one of the 6 lives.
The player continues guessing letters until either:
All letters are correctly guessed (the player wins), or
The player runs out of lives (the player loses).
The player will be notified after each guess whether they’ve won or lost a life.
Project Files:
hangman.py - The main script that runs the game logic.
hangman_words.py - This file contains the word_list variable, a list of potential words the game will randomly choose from.
hangman_art.py - This file contains:
stages variable, which holds ASCII art representations of the hangman for each life stage.
logo variable, which holds the game logo as ASCII art.
Game Rules:
The player is allowed 6 incorrect guesses (represented by 6 lives).
The game ends when:
The player guesses all letters correctly, or
The player runs out of lives.
The player cannot guess the same letter more than once (repeated guesses will prompt a message but won’t affect lives).
Example Game Flow:
Initial Display:

markdown
Copy code
Word to guess: _ _ _ _ _
****************************6 LIVES LEFT****************************
Player Guess:

yaml
Copy code
Guess a letter: e
Word to guess: _ e _ _ e
Incorrect Guess:

markdown
Copy code
Guess a letter: x
You guessed x, that's not in the word. You lose a life.
****************************5 LIVES LEFT****************************
Winning:

markdown
Copy code
****************************YOU WIN****************************
Losing:

markdown
Copy code
You guessed f, that's not in the word. You lose a life.
***********************YOU LOSE**********************
The correct word is apple.
Setup Instructions:
Python Version: Ensure you have Python 3.x installed.
Dependencies: This project doesn't require any third-party libraries.
Running the Game: Run the game by executing hangman.py in your terminal or Python environment.
bash
Copy code
python hangman.py
Future Enhancements:
Add more words to word_list for variety.
Implement difficulty levels (easy, medium, hard) by changing word lengths or allowed lives.
Add a graphical interface using libraries like tkinter or pygame.
Enjoy the game!
