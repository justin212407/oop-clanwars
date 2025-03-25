# OOP based RPG Game with TypeScript

#### Description

A TypeScript project demonstrating Object-Oriented Programming (OOP) principles using a fantasy game simulation. It
includes classes like `Player`, `GameSession`, `Creature`, and interfaces like `Combatant`, `Healer`, `Hero`, `Villain`.


# Install dependencies
pnpm install
```

```bash
# To start the application
pnpm start

# To build the application
pnpm run build

# To serve the built application
pnpm run serve
```

#### Features

- Implementation of OOP concepts in TypeScript.
- Game simulation with player interactions and game session management.
- Extendable architecture for adding more player types and actions.

#### Code Structure

- `src/`: Source code directory.
  - `index.ts`: Entry point of the application.
  - `interfaces/`: Definitions of interfaces like `Combatant`, `Healer`.
  - `models/`: Game models like `Player`, `GameSession`.
- `tsconfig.json`: TypeScript configuration file.
- `package.json`: Project metadata and dependencies.

### Object-Oriented Architecture Explanation

#### Core Concepts

##### Classes

- **Player**: Represents a generic player in the game. Inherits from `Creature` and has properties
  like `name`, `health`, and `level`. It also includes methods like `attack()` and `defend()`.
- **Creature**: An abstract class that serves as a base for `Player` and `Animal`. It includes methods
  like `makeSound()` and `locate()`.
- **Animal**: Extends `Creature`. Represents animals in the game with health properties and methods.
- **GameSession**: Manages the game's state, including player lists and game status. It uses singleton pattern for
  global access.

##### Inheritance

- **Inheritance**: Demonstrated by `Player`, `Knight`, `Priest`, `Archer`, `Witch`, and `Animal`, which inherit
  from `Creature`. This allows for shared functionalities and properties.

##### Interfaces

- **Combatant, Healer, Hero, Villain**: Interfaces that define specific actions
  like `fight()`, `heal()`, `performHeroicAction()`, and `performEvilDeed()`. Implemented by different player types to
  ensure diverse capabilities.

##### Encapsulation

- Properties like `name` in `Player` and `Animal` are marked as readonly, and health is encapsulated with getter and
  setter methods, illustrating encapsulation.

#### Design Patterns

- **Singleton**: Used in `GameSession` to ensure only one instance of the game session exists.
- **Strategy Pattern**: Demonstrated by implementing interfaces on different player types, allowing them to change their
  behavior (like fighting or healing) dynamically.

#   o o p - c l a n w a r s  
 