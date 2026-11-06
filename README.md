# Fantasy Heroes Mini-System (Python OOP Project)

## Project Description

This project is a simple object-oriented (OOP) text-based fantasy battle system implemented in **Python 3**.
It demonstrates the use of classes, inheritance, polymorphism, encapsulation, and object interaction.

The system includes heroes, monsters, items, an inventory, and a basic battle simulation executed from `main.py`.

---

## Implemented Classes

### Base Class

**Character** (`character.py`)

Attributes:

* `name` — character name
* `health` — current health points
* `attack_power` — attack strength

Methods:

* `attack(target)` — deals damage to another character
* `take_damage(amount)` — reduces health (cannot go below 0)
* `is_alive()` — returns True if health > 0
* `__str__()` — string representation of character status

---

## Hero Classes (`heroes.py`)

### Warrior

Special feature:

* Has a chance to perform a **critical hit** (double damage)

### Mage

Special feature:

* Uses **mana** to cast stronger attacks
* If mana is insufficient, performs a normal attack

---

## Monster Classes (`monster.py`)

### Monster

Base monster class.

### Goblin

Special feature:

* Has a chance to **dodge attacks**

### Zombie

Special feature:

* Can **resurrect once** after being defeated

---

## Item Classes (`item.py`)

### Item

Base item class.

### HealthPotion

Effect:

* Restores character health

### Sword

Effect:

* Increases character attack power

---

## Inventory (`inventory.py`)

The Inventory class allows characters to:

* Store items
* List items
* Use items by name
* Remove used items automatically

---

## How to Run the Program

1. Open terminal in the project folder.

2. Run the command:

```bash
python main.py
```

3. The battle simulation will start and results will be printed to the console.

---

## Example Program Output

Example output may look like this:

```
Sword added to inventory.
Health Potion added to inventory.

--- BATTLE STARTS ---

Arthur attacks Sneaky Goblin for 15 damage.
Sneaky Goblin attacks Merlin for 8 damage.
Merlin uses Health Potion and restores 20 health.
Merlin casts a spell! Mana left: 40.
Arthur attacks Sneaky Goblin for 15 damage.

--- FINAL STATUS ---

Arthur | HP: 100 | ATK: 15 | Status: Alive
Merlin | HP: 92 | ATK: 10 | Status: Alive
Sneaky Goblin | HP: 0 | ATK: 8 | Status: Defeated
```

Note: The exact numbers may vary due to randomness (critical hits and dodging).

---

## Technologies Used

* Python 3
* Object-Oriented Programming (OOP)
* No external libraries

---

## Key OOP Concepts Demonstrated

* Classes and objects
* Inheritance
* Method overriding (polymorphism)
* Encapsulation
* Object interaction
* Code modularity

---

## Project Structure

```
fantasy_game/

character.py
heroes.py
monster.py
item.py
inventory.py
main.py
README.md
```

---

## Author

Student project demonstrating basic OOP design and implementation in Python.
