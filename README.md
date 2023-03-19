# Hangman-Game

The goal of the project is to create a command-line Hangman game where the player has to guess the letters of a randomly selected secret word. The player has a limited number of guesses, and for each incorrect guess, a part of a hangman figure is drawn. The player wins if they can correctly guess the entire word before the hangman figure is completed. 


## Instructions to run the game

* Open the Github repository where the game code is hosted.

* Click on the green "Code" button and then select "Download ZIP" to download the code as a ZIP file.

* Extract the ZIP file to a folder on your computer.

* Open a command prompt or terminal window and navigate to the folder where you extracted the code.

* Type ```python hangman.py``` and press Enter to start the game.

* Follow the prompts to play the game.

## Functionality of the code

* The code imports the random module to choose a random word from a pre-defined list of animals.

* The code defines a variable hang, which is a list of strings. Each string represents a level of the Hangman game, with increasing complexity as the number of incorrect guesses increases.

* The code defines a function getRandomWord() which selects a random word from a list of pre-defined words.

* The code defines a function displayBoard() which prints the current status of the game, including the picture of the Hangman, missed letters, and the secret word with blank spaces for unguessed letters.

* The code defines a function getGuess() which takes user input to get a single letter guess, checking for invalid input and previously guessed letters.

* The code defines a function playAgain() which prompts the user to play again and returns True or False depending on the user's input.

* The code initializes the variables missedLetters, correctLetters, secretWord, and gameIsDone.

* The code runs a while loop that continues to display the current status of the game and prompt the user for a guess until the game is either won or lost. If the user guesses a correct letter, the code updates the correctLetters variable and checks if the user has won the game. If the user guesses an incorrect letter, the code updates the missedLetters variable and checks if the user has lost the game. If the game is over, the code calls the playAgain() function to ask if the user wants to play again. If the user chooses to play again, the code resets the game variables and chooses a new secret word. If the user chooses not to play again, the while loop is broken and the program terminates.
