# Python-Slot-Machine
Slot Machine Game
This Python script is a simple text-based slot machine game.

How it works
The game starts by asking the user to deposit an amount of money. This is done in the deposit function which keeps asking the user for an amount until a positive integer is entered.

The main function is the entry point of the game. It first calls the deposit function to get the initial balance. Then it enters a loop where it keeps running the game until the user decides to quit or the balance becomes 0.

In each round of the game, the spin function is called. This function first asks the user how many lines they want to bet on and how much they want to bet on each line. It then generates a random slot machine spin using the get_slot_machine_spins function and calculates the winnings using the check_winnings function.

The get_slot_machine_spins function generates a random spin of the slot machine. It does this by creating a list of symbols based on the symbol_count dictionary and then randomly selecting symbols for each column of the slot machine.

The check_winnings function checks if the user has won anything. It does this by checking each line the user has bet on and seeing if all the symbols on that line are the same. If they are, the user wins a certain amount based on the value of the symbol and the amount they bet.

If the balance becomes 0, the user is asked if they want to deposit more money. If they choose to do so, the deposit function is called again to add more money to the balance.

The game continues until the user decides to quit or the balance becomes 0 and the user chooses not to deposit more money. At the end, the final balance is printed.

How to run
To run the game, simply execute the script in a Python environment:
python app.py

Requirements
This script requires Python 3.6 or later. No additional libraries are needed.
