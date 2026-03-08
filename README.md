# Number Guessing Game

This is a simple Python number guessing game.

```python
import random

number_to_guess = random.randint(1, 10)
tries = 3

while tries > 0:
    guess = int(input("Enter your guess: "))
    if guess == number_to_guess:
        print("You guessed it!")
        break
    elif guess < number_to_guess:
        print("Too low!")
    else:
        print("Too high!")
    tries -= 1
