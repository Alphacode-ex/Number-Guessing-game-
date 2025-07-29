# Number-Guessing-game-
By running this Python code you will there is a number Guessing game as an output

#Generates random number between 1 and 100
import random
n = random.randint(1,100)
a = -1
guesses = 0

#loop until the user gusses the correct number 
while(a != n):
    guesses +=1
    a= int(input("Guess the number : "))
    if(a>n):
        print("Lower number please" )
    else:
        print("Higher number please")

print(f"You have guessed the number {n} correctly in {guesses} attempt")
