# Number-Guessing-game-
By running this Python code you will there is a number Guessing game as an output

#
import random

n = random.randint(1, 100)
guesses = 0  # Initialize guess counter

while True:
    try:
        a = int(input("Guess the number: "))
        guesses += 1

        if a > n:
            print("Lower number please")
        elif a < n:
            print("Higher number please")
        else:
            print(f"You have guessed the number {n} correctly in {guesses} attempts")
            break
    except ValueError:
        print("Please enter a valid number")
