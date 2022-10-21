# WASM Rust Tutorial

## Setup

This section describes how to set up the toolchain for compiling Rust programs to WebAssembly and integrate them into JavaScript.

### 1. The `Rust Toolchain`

We will need the standard Rust toolchain, including `rustup`, `rustc`, and `cargo`.

> Follow the instructions to install the Rust toolchain [here](https://www.rust-lang.org/tools/install).

The Rust and WebAssembly (WASM) experience is riding the Rust release trains to stable! That means we don't require any experimental feature flags. However, we do require Rust 1.30 or newer.

### 2. The `Wasm Pack` 

The `wasm-pack` is our one-stop shop for building, testing, and publishing Rust-generated WebAssembly (WASM).

Get the `wasm-pack` [here](https://rustwasm.github.io/wasm-pack/installer/)!

### 3. The `Cargo Generate`

The [`cargo-generate`](https://github.com/cargo-generate/cargo-generate) helps you get up and running quickly with a new Rust project by leveraging a pre-existing git repository as a template.

Install `cargo-generate` with this command:
```rust
cargo install cargo-generate
```

### 4. The `NPM`

The `npm` is a package manager for JavaScript. We will use it to install and run a JavaScript bundler and development server. At the end of the tutorial, we will publish our compiled `.wasm` to the `npm` registry.

Follow [these](https://docs.npmjs.com/getting-started) instructions to install `npm`.

If you already have `npm` installed, make sure it is up to date with this command:

```
npm install npm@latest -g
```