# Number Guessing Game

A simple command-line number guessing game written in Rust. This project is an introductory exercise from *The Rust Programming Language* book, and is designed to familiarize beginners with fundamental Rust concepts, such as handling user input, using external crates, and implementing loops and conditional logic.

## Overview

In this game, the program randomly selects a secret number between 1 and 100, and the player tries to guess it. After each guess, the program provides feedback indicating whether the guess is too low, too high, or correct. The game continues until the player correctly guesses the number.

## Features

- **Random Number Generation**: The program uses the `rand` crate to generate a random secret number.
- **Input Handling**: The program reads and validates user input from the command line.
- **Feedback on Guesses**: After each guess, the program provides feedback on whether the guess was too low, too high, or correct.

## Getting Started

### Prerequisites

- [Rust](https://www.rust-lang.org/tools/install) should be installed on your system.

### Running the Game

1. Clone this repository:

    ```sh
    git clone https://github.com/imaazkhalid/guessing-game.git
    cd number-guessing-game
    ```

2. Build and run the program with `cargo`:

    ```sh
    cargo run
    ```

3. Follow the on-screen instructions to enter your guesses.

## How to Play

1. When the game starts, it will print "Guess the number!".
2. Enter a guess when prompted. The program will validate your input and notify you if it’s invalid.
3. After each valid guess, the program will respond:
   - **"Too small!"** if the guess is lower than the secret number.
   - **"Too big!"** if the guess is higher than the secret number.
   - **"You win!"** if the guess matches the secret number, ending the game.
4. Continue guessing until you find the correct number!

### Example Gameplay

```plaintext
Guess the number!
Please input your guess.
50
You guessed: 50
Too small!

Please input your guess.
75
You guessed: 75
Too big!

Please input your guess.
63
You guessed: 63
You win!
```

## Project Structure

- **`src/main.rs`**: Contains all game logic, including random number generation, user input handling, and feedback based on guesses.

## Learning Highlights

This project is designed to help you practice and learn about:
- **Using external crates**: The `rand` crate for random number generation.
- **Handling standard input/output**: Accepting and validating user input.
- **Control flow**: Using loops and `match` statements for decision-making.
- **Error handling**: Managing input parsing errors gracefully.

---

This project is a fun and interactive way to start learning Rust. Feel free to experiment with the code, add more features, or adjust the game mechanics as you continue your Rust journey!