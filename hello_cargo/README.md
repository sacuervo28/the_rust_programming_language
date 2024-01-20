# Hello, Cargo

- Cargo projects can be created with `cargo new proyect_name`
- Git files won't be generated if we're using cargo inside a git repository
- `Cargo.toml` is the cargo configuration file

## Building and running

- A non cargo proyect can be made into a cargo one by following these steps:
    1. Inside the proyect directory add a cargo.toml file with the appropriate settings
    2. Add an src folder and move your proyect files in there (non-proyect files should go outside)
- You may build and compile your cargo proyects in two ways:
    1. `cargo build` + `./target/debug/hello_cargo`
    2. Just using `cargo run`
- `cargo check` compiles the code but doesn't generate an executable
- You may want to use `cargo check` just to make sure your code will compile. When you actually want to run your program, you use `cargo run`.

## Building for release

- `cargo build --release` will compile your program with optimizations and generate the executable at ./target/release. 
- This command should be used for benchmarking our programs
