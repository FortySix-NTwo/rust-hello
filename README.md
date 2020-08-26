# Rust Installing & Setup

> Rust for MacOS

---

## Step 1

Copy the following command into the terminal

```bash
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh

# Source the binaries within your ~/.zshrc | ~/.bashrc
source $HOME/.cargo/env

# Verify that all has installed correctly
rustup toolchain list

# for the version
rustup --version

# to update
rustup update
```

## Step 2

Creating a new Project in rust

```bash
# within the terminal run
cargo new project-name

# Which will generate a new project with the following structure

# \- project-name
# |- Cargo.toml
# |- src
#   |- main.rs
```

## Cargo.toml

is the manifest file for Rust. It’s where you keep metadata for your project, as well as dependencies.

## src/main.rs

is our main code file for the application

## cargo new command

generates a "Hello, world!" project for us! We can run this program by moving into the new directory that we made with the following command

```bash
# Generate hello-world
cargo new

# running program
cargo run
```

## Adding dependencies

Like [NPMjs.com](http://npmjs.com) rust provides us with [crates.io](http://crates.io/), to add a dependence we can add it to the Cargo.toml file as follows:

```bash
# Cargo.toml

[dependencies]
dependency-name = "1.0"
```

### Compiling our dependency

we will have to run the following command

```bash
cargo build
```

You’ll see that running this command created a new file for us, Cargo.lock. This file is a log of the exact versions of the dependencies we are using locally.

## Step 3

Run the application by typing the following into the terminal

```bash
cargo run
```

and wait for the magic 🎩

### VSCode Extension

we can install a rust-lang vscode extension at the following link

[https://marketplace.visualstudio.com/items?itemName=rust-lang.rust](https://marketplace.visualstudio.com/items?itemName=rust-lang.rust)
