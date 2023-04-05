# Pokemon Battle Simulator

This Python program allows users to simulate a Pokemon battle between two trainers. It features a simple turn-based battle system, where Pokemon can attack each other, gain and lose health, and trainers can use potions or switch their active Pokemon.

## Features

- Create and initialize Pokemon with a name, type, and level.
- Pokemon gain and lose health during battles.
- Pokemon can get knocked out or revived.
- Trainers can use potions to restore their Pokemon's health.
- Trainers can switch their active Pokemon during battles.
- A simple turn-based battle system based on the Pokemon's type and level.

## Usage

To start a battle simulation, run the script and follow the prompts to enter the names of the two trainers and choose their Pokemon. The program will then simulate a battle between the trainers and display the results of each action taken during the battle.

## Classes

- `Pokemon`: Represents a Pokemon, with attributes such as name, level, health, max health, type, and knockout status.
- `Trainer`: Represents a trainer, with attributes such as a list of Pokemon, number of potions, the current active Pokemon, and a name.

## Example

```python
# Create Pokemon
charmander = Pokemon("Charmander", "Fire", 7)
squirtle = Pokemon("Squirtle", "Water")

# Create Trainers
trainer_one = Trainer([charmander], 3, "Ash")
trainer_two = Trainer([squirtle], 3, "Gary")

# Battle Simulation
trainer_one.attack_other_trainer(trainer_two)
trainer_two.attack_other_trainer(trainer_one)
trainer_two.use_potion()
trainer_one.attack_other_trainer(trainer_two)
trainer_two.switch_active_pokemon(0)
trainer_two.switch_active_pokemon(1)
```
## Disclaimer

Please note that the code is not optimized for a full-fledged game or application and serves as a basic example of a Pokemon battle simulation. Feel free to expand on this code and customize it to your needs.
