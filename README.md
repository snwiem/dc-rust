# dc-rust

DevContainer for Rust Development

## Usage

After creating your project directory checkout this DevContainer specification by

```bash
git submodule add https://github.com/snwiem/dc-rust.git .devcontainer
```

You need to rebuild the container. Either you can use `Ctrl+Shift+P` and select `Dev Containers: Reopen....` or you can just open the project folder with `code .` and code will ask you to reopen the project in a container.

After the container is spun up you can check that the rustup environment is available by checking

```bash
rustc --version
```

If this is working just initialize the project using

```bash
cargo init [--bin|--lib] [--name "Other than current directory"]
```

Now start developing your next fancy rust application.

## Maintainance

To update the container definition use

```bash
cd .devcontainer
git checkout main
git pull --all
```

You need to rebuild the container after that.
