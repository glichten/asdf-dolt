# asdf-dolt

[Dolt](https://github.com/dolthub/dolt) plugin for the [asdf version manager](https://asdf-vm.com).

## Note on System-Wide Usage

Dolt often runs as a long-lived SQL server (`dolt sql-server`) and may be
started by daemons, launchd services, or tools like
[Gas Town](https://github.com/steveyegge/gastown) outside of your login shell.
asdf shims depend on shell initialization and may not resolve in those contexts.

**If you use Dolt as a background server or with Gas Town, [Homebrew](https://brew.sh)
is the recommended install method** (`brew install dolt`). This plugin is still
useful for CI environments, testing specific versions, or systems without
Homebrew.

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
