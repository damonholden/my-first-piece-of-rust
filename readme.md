# My First Piece Of Rust

This project is the first piece of rust I've written.

## Rust Install

Rust was installed on my Windows machine using the Rustup installer [downloaded
from this
link](https://static.rust-lang.org/rustup/dist/x86_64-pc-windows-msvc/rustup-init.exe).

After installation finished, I checked if Rust was up-to-date using the shell
command `rustup update`.

## VSCode Setup

Rust officially supports a single VSCode extension - Rust-analyzer, which features:

- code completion with imports insertion
- go to definition, implementation, type definition
- find all references, workspace symbol search, symbol renaming
- types and documentation on hover
- inlay hints for types and parameter names
- semantic syntax highlighting
- and more

[The Rust-analyzer VSCode extension can be found using this
link.](https://marketplace.visualstudio.com/items?itemName=rust-lang.rust-analyzer)

## hello-rust Project setup

The 'hello-rust' project was setup by running the following shell command:

```lang-bash
cargo new hello-rust
```

This command creates a new rust hello-world project in a directory called
`hello-world`. The program code should look something like this:

```lang-rust
fn main() {
  println!("Hello, world!");
}
```

Moving into the new directory, the Rust program can be run by
executing the following command:

```lang-bash
cargo run
```

The output will be something similar to the following:

```lang-bash
$ cargo run
   Compiling hello-rust v0.1.0 (/Users/ag_dubs/rust/hello-rust)
    Finished dev [unoptimized + debuginfo] target(s) in 1.34s
     Running `target/debug/hello-rust`
Hello, world!
```

## Adding Dependencies

Dependencies are included to a project by appending to the dependencies list in
the `Cargo.toml` file.

For example the ferris-says dependency was added by appending the following to
the `Cargo.toml` file:

```lang-toml
[dependencies]
ferris-says = "0.2"
```

## Sources

[This project was created following the official Rust "Getting Started"
documentation, which can be found
here.](https://www.rust-lang.org/learn/get-started)

[Documentation for Cargo - the Rust package manager can be found
here](https://doc.rust-lang.org/cargo/index.html).
