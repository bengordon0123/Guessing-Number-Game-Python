
import random

total = 0

my_number = random.randint(1, 201)

name = input("Enter your name: ")
print(name, ",Can you guess the number I’m thinking of? It’s between 1 and 200.")

while total < 10:
    guess = int(input("Enter your guess: ", ))

    total = total + 1

    if guess < my_number:
        print("The number I’m thinking of is higher.")

    if guess > my_number:
        print("The number I’m thinking of is lower.")

    if guess == my_number:
        total = str(total)
        print("Good job, " + name+ " you guessed my number in, " + total+ " attempts.")
        break
