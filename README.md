# asdf-dolt

[Dolt](https://github.com/dolthub/dolt) plugin for the [asdf version manager](https://asdf-vm.com).

## Dependencies

- `bash`, `curl`, `tar`, `git`: generic POSIX utilities

## Install

```shell
asdf plugin add dolt https://github.com/glichten/asdf-dolt.git
```

## Usage

```shell
# Show all installable versions
asdf list all dolt

# Install a specific version
asdf install dolt latest

# Set a version globally
asdf set --home dolt latest

# Check current version
dolt version
```

## License

See [LICENSE](LICENSE).
