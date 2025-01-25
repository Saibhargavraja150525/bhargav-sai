code has not found 
from termcolor import colored
from colorama import init

# Initialize colorama
init()

# List of rainbow colors
rainbow_colors = ['red', 'yellow', 'green', 'cyan', 'blue', 'magenta']

# Text to display
text = "RAINBOW CODE IN PYTHON"

# Print each letter in a rainbow color
for i, letter in enumerate(text):
    if letter != " ":
        color = rainbow_colors[i % len(rainbow_colors)]  # Cycle through colors
        print(colored(letter, color), end="")
    else:
        print(" ", end="")  # Preserve spaces
print()
