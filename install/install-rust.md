# Install Rust Programming Language

1. add the following into `.profile` or `.bash_profile`:
```bash
export CARGO_HOME="$XDG_DATA_HOME/cargo"
export RUSTUP_HOME="$XDG_DATA_HOME/rustup"
export PATH="$CARGO_HOME/bin:$PATH"
```
2. Source `.profile` or `.bash_profile` with the following:
```bash
$ ~ source .profile
```
2. run the following code into terminal:
```bash
$ curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```
3. Just accept the basic until it finish.
4. Check if rust already install correctly by with the following:
```bash
$ ~ $ cargo version
cargo 1.68.2 (6feb7c9cf 2023-03-26)
```
if the version is appear, then we are successfuly installing rust

**NOTES:**

- `$CARGO_HOME` and `$RUSTUP_HOME` that we add into `.profile` or `.bash_profile` is from [archlinux base dir](https://wiki.archlinux.org/title/XDG_Base_Directory).
- Curl command that we run is from official [rust website](https://www.rust-lang.org/tools/install)
