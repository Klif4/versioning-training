# Installing Cocogitto on Ubuntu

Cocogitto is typically installed on Ubuntu using Rust's package manager, Cargo, as the tool is written in Rust.

Here is the recommended method, step-by-step:

## 1. Install Rust and Cargo
You must first install Rust and its package manager Cargo (if you haven't already). This is the simplest way to get the latest version of Cocogitto.

Install necessary dependencies:

```bash
sudo apt update
sudo apt install build-essential curl
Install Rust via rustup:
```


```bash
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
Follow the on-screen instructions. It is usually recommended to choose the default option (1).
```

### Activate Cargo:

Close and reopen your terminal, or run this command to load Cargo's environment variables into your current session:


```bash
source $HOME/.cargo/env
```

## 2. Install Cocogitto
Once Cargo is installed, you can install Cocogitto directly from crates.io (the Rust package repository).

Start the installation:


```bash
cargo install --locked cocogitto
```

The --locked option ensures that the dependency versions specified in Cocogitto's Cargo.lock file are used, making the installation more reliable.

## 3. Verify the Installation
After installation, verify that the executable cog (the name of the Cocogitto command) is accessible:


```bash
cog --version
```
