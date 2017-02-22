
import random

total = 0

my_number = random.randint(1, 201)

name = input("Enter your name: ")
print(name, ",Can you guess the number I’m thinking of? It’s between 1 and 200.")

if total == 10:

print(name, ", you're all out of guesses! Try again next time!")

while total < 10:
    guess = int(input("Enter your guess: ", ))

    total = total + 1

    elif guess < my_number:
        print("The number I’m thinking of is higher.")

    elif guess > my_number:
        print("The number I’m thinking of is lower.")

    elif guess == my_number:
        total = str(total)
        print("Good job, " + name+ " you guessed my number in, " + total+ " attempts.")
        break
        
        
