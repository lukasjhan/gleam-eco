# Gleam-Eco

Gleam-Eco is a development environment setup for working with Gleam, Erlang, and Elixir using Nix. This project aims to provide a consistent and reproducible development environment for BEAM-based languages, with a focus on Gleam.

## Prerequisites

- Nix package manager installed on your system. If you haven't installed Nix yet, you can do so by following the instructions at [nixos.org](https://nixos.org/download.html).

## Getting Started

1. Clone this repository:

   ```
   git clone https://github.com/lukasjhan/gleam-eco.git
   cd gleam-eco
   ```

2. Enter the Nix shell:

   ```
   nix-shell
   ```

   This command will download and set up the required dependencies (Erlang, Elixir, and Gleam) in an isolated environment.

3. Once in the Nix shell, you can start using Gleam, Erlang, and Elixir.

## Usage

### Gleam

To create a new Gleam project:

```
gleam new my_project
cd my_project
```

To run your Gleam project:

```
gleam run
```

### Erlang

To start an Erlang shell:

```
erl
```

### Elixir

To start an Elixir interactive shell (IEx):

```
iex
```

## Project Structure

- `shell.nix`: This file defines the Nix environment, including the versions of Erlang, Elixir, and Gleam to be used.

## Customization

You can modify the `shell.nix` file to change the versions of Erlang, Elixir, or Gleam, or to add additional dependencies to your development environment.

## Benefits of This Setup

- **Reproducibility**: Anyone with Nix installed can reproduce the exact same development environment.
- **Isolation**: The development environment is isolated from your system packages, preventing conflicts.
- **Version Control**: The development environment configuration can be version-controlled along with your project code.

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is open source and available under the [MIT License](LICENSE).

---

Happy coding with Gleam, Erlang, and Elixir!
