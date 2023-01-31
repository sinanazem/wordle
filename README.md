# Wordle

<img src="https://assets2.rockpapershotgun.com/wordle-past-answers-header.jpg/BROK/thumbnail/1200x630/wordle-past-answers-header.jpg" width=550>

Wordle is a word game, which recently got very popular and was added to NYT Games website. It is developed by Josh Wardle. You can find the original game here. However, you can only play it once a day.

Luckily, in this version of Wordle that you are going to be programming, you will be able to play as many times as you want in a day. Moreover, you will be allowed to see which words could potentially be the right answer. What is more, you will be using a bigger data set than the actual Wordle, which basically involves all the 5 letter words in a Scrabble dictionary.


## Rules
- The player enters a random 5-letter word.
- If the random word is the word to be guessed, the game is over. The player receives a congratulations message.
- If the random word isn’t the word to be guessed, the player is informed about whether the right letter is at the right place and if some of the letters are in the word - but wrongly placed.<br>
- Based on this, the player has 6 tries to guess the word.
- At the end of the 6 attempts, if the player fails to guess the right word, the word is revealed.<br>

## TODO
- Read the possible words from the txt file and save them on a list.
- Make sure that the user can enter input exactly 6 times.
- Make sure that regardless of the case, the input is processed correctly.
- Make sure that you use appropriate data structures for valid characters, invalid positions, and invalid characters.
- Use the random module to make sure the word to be guessed is randomly chosen.
- Cluster the potential words accordingly and reveal it to the player each round.
- In case the player first guesses the right letter at the wrong place, and later on gets the place right, remove that from your valid characters invalid positions.

## Tips
- At the very beginning each of the words have a chance of being the word to be guessed.
- A word is invalid, when there are invalid letters in it or when there is a valid letter at the wrong place.
- A word is possible, when it isn’t invalid and contains the correctly guessed letter at the right place.
 -You can initiate a random number by:
```
from random import randint, seed
seed()
```
