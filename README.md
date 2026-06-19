# Easybrain Solver

A high-performance algorithmic solver for an Easybrain iPhone puzzle game, written in Rust. This command-line tool processes text-based game states and computes the optimal solution or next moves to help you clear the board.

## 📖 About the Project

Easybrain develops numerous popular logic puzzles for iOS. This repository provides an automated solver tailored to read a game's state directly from a text file and output the winning solution. Built entirely in Rust, it ensures memory safety and rapid execution, even for complex board calculations.

## 🗂 Project Structure

* `src/`: Contains the Rust source code and core logic for the solver.
* `input`: The default configuration file representing the current game board or puzzle state.
* `input.2` / `input.bak`: Alternative or backup puzzle states for testing different scenarios.
* `input.explained`: Documentation outlining how to properly format your custom puzzle states.
* `Cargo.toml`: Rust package manager and dependency configuration.

## ⚙️ Prerequisites

You will need the Rust toolchain installed to compile and run this project. If you don't have it, install it via `rustup`:

    ```bash
    curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh

## 🚀 Installation

Clone the repository to your local machine and build the project using Cargo:

    ```bash
    git clone https://github.com/rmruiz/easybrain.git
    cd easybrain
    cargo build --release

## 💡 Usage

The solver reads the puzzle configuration from the local input files. To understand how to map the game from your iPhone screen into text, check the input.explained file.

To run the solver using the default input file:

    ```bash
    cargo run --release

If your code supports passing file arguments, you can test other configurations like this:

    ```bash
    cargo run --release -- input.2

## 📝 How to Use

Open the target Easybrain game on your iPhone.

Replicate the game grid, numbers, or current state inside the input file according to the formatting rules in input.explained.

Execute the solver.

Follow the output in your terminal to progress in your game.

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to check the issues page if you want to contribute, optimize the algorithms, or add support for other Easybrain games.

##  📄 License
This project is open-source and available under the MIT License.
