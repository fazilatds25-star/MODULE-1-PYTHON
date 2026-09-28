# MODULE-1-PYTHON
import random

def roll_dice():
    # Generate a random number between 1 and 6
    return random.randint(1, 6)

print("🎲 Welcome to the Python Dice Rolling Simulator! 🎲\n")

while True:
    # Get user choice and clean it up (lowercase and strip spaces)
    user_input = input("Roll the die? (y/n): ").strip().lower()
    
    if user_input == 'y':
        result = roll_dice()
        print(f" Let it roll... You got a: {result}!\n")
    elif user_input == 'n':
        print("Thanks for playing! Goodbye. 👋")
        break
    else:
        print("Invalid input. Please enter 'y' for Yes or 'n' for No.\n")
