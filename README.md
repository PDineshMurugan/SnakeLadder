# Snake and Ladder Game

A simple console-based Snake and Ladder game implemented in Java. This game allows two players to compete by rolling a dice and moving their pieces on a board filled with snakes and ladders.

## Table of Contents

- [Features](#features)
- [How to Play](#how-to-play)
- [Setup and Installation](#setup-and-installation)
- [Gameplay](#gameplay)
- [Board Layout](#board-layout)
- [Time and Space Complexity](#time-and-space-complexity)
- [Contributing](#contributing)
- [License](#license)

## Features

- Two-player mode.
- Random dice rolls.
- Ladders that move players up.
- Snakes that move players down.
- Simple text-based user interface.
- Board implemented using arrays.

## How to Play

1. Each player takes turns to roll the dice by pressing the Enter key.
2. The player moves forward by the number of spaces indicated by the dice roll.
3. If a player lands on a ladder, they move up to the ladder's end.
4. If a player lands on a snake, they move down to the snake's tail.
5. The first player to reach exactly 100 wins the game.

## Setup and Installation

1. Clone the repository:

```sh
git clone https://github.com/PDineshMurugan/snake-ladder-game.git
```

2. Navigate to the project directory:

```sh
cd snake-ladder-game
```

3. Compile the Java program:

```sh
javac Snake_Ladder/Snake_Ladder.java
```

4. Run the game:

```sh
java Snake_Ladder/Snake_Ladder
```

## Gameplay

### Example of a game session

```plaintext
Player 1 Enter your name:
Alice
Player 2 Enter your name:
Bob
Alice
Roll the dice by pressing Enter 
The dice rolled: 4
Position of Alice: 4
___________________________________________
Bob
Roll the dice by pressing Enter 
The dice rolled: 5
Position of Bob: 5
___________________________________________
...
*******************************
*                             *
*     Winner is Alice         *
*                             *
*******************************
```

## Board Layout

The board consists of 100 squares with some squares containing ladders and snakes. Landing on a ladder moves the player up, while landing on a snake moves the player down. Here is the layout of ladders and snakes:

### Ladders

- 2 -> 38
- 7 -> 14
- 8 -> 31
- 15 -> 26
- 21 -> 42
- 28 -> 84
- 36 -> 44
- 51 -> 67
- 71 -> 91
- 78 -> 98
- 87 -> 94

### Snakes

- 16 -> 6
- 46 -> 25
- 49 -> 11
- 62 -> 19
- 64 -> 60
- 74 -> 53
- 89 -> 68
- 92 -> 88
- 95 -> 75
- 99 -> 80

## Time and Space Complexity

### Time Complexity

- **Initialization**: Initializing the board with snakes and ladders takes O(1) time as it involves a fixed number of assignments.
- **Dice Roll**: Each dice roll operation is O(1).
- **Movement**: Moving a player involves a fixed number of operations to check the board and update the player's position, hence O(1).

### Space Complexity

- **Board**: The board is represented by an array of size 101, which takes O(101) space, simplified to O(1) as it is a constant.
- **Players**: Storing the positions of two players requires O(2) space, which is also O(1).

Overall, the time complexity per move is O(1), and the space complexity of the game is O(1).

## Contributing

Contributions are welcome! If you find any issues or have suggestions for improvements, feel free to open an issue or submit a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.
