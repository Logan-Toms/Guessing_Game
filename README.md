# Guess the Number Game in Rust

This repository contains a simple command-line "Guess the Number" game, implemented in Rust. The program selects a random number between 1 and 100, and the player must guess it by providing inputs. After each guess, the program will give feedback indicating whether the guess was too high, too low, or correct.

This project was developed by following the tutorial guide in [*The Rust Programming Language* book](https://doc.rust-lang.org/book/), often referred to as *The Rust Book*, specifically using the instructions provided to build an interactive CLI guessing game.

## How to Play

1. Clone the repository and navigate into it:
   ```bash
   git clone https://github.com/Logan-Toms/Guessing_Game.git
   cd guess-the-number
   ```

2. Compile the program:
   ```bash
   cargo build --release
   ```

3. Run the program:
   ```bash
   cargo run
   ```

4. Follow the on-screen instructions to enter your guesses.

## How it Works

- The program generates a random number between 1 and 100 using the `rand` crate.
- It then enters a loop where it:
- Prompts the player to enter a guess.
- Parses the guess and provides feedback:
    - "Too small!" if the guess is less than the secret number.
    - "Too big!" if the guess is more than the secret number.
    - "You win!" if the guess matches the secret number.
- The game ends once the correct number is guessed.

## Dependencies

- **rand**: A Rust crate used for generating random numbers. Ensure this crate is added to your `Cargo.toml`.

## Acknowledgments

This project follows the "Guessing Game" project guide from *The Rust Programming Language* book, which provides an excellent introduction to Rust's standard library, error handling, and basic concepts.

## License

This project is licensed under the MIT License.