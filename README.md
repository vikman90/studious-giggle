# Wazuh Agent Documentation Demo

This is a temporary PoC: https://vikman90.github.io/studious-giggle

## Setup

### Requirements

- mdbook

```shell
apt install cargo
cargo install mdbook
export PATH=$PATH:$HOME/.cargo/bin
```

### Build documentation

```shell
mdbook build
```

### Serve documentation

```shell
mdbook serve
```

This will make documentation available at http://127.0.0.1:3000.
