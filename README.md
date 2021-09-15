<div align="center">

# asdf-syft [![Build](https://github.com/davidgp1701/asdf-syft/actions/workflows/build.yml/badge.svg)](https://github.com/davidgp1701/asdf-syft/actions/workflows/build.yml) [![Lint](https://github.com/davidgp1701/asdf-syft/actions/workflows/lint.yml/badge.svg)](https://github.com/davidgp1701/asdf-syft/actions/workflows/lint.yml)


[syft](https://github.com/anchore/syft) plugin for the [asdf version manager](https://asdf-vm.com).

</div>

# Contents

- [Dependencies](#dependencies)
- [Install](#install)
- [Why?](#why)
- [Contributing](#contributing)
- [License](#license)

# Dependencies

- `bash`, `curl`, `tar`: generic POSIX utilities.
- `SOME_ENV_VAR`: set this environment variable in your shell config to load the correct version of tool x.

# Install

Plugin:

```shell
asdf plugin add syft
# or
asdf plugin add syft https://github.com/davidgp1701/asdf-syft.git
```

syft:

```shell
# Show all installable versions
asdf list-all syft

# Install specific version
asdf install syft latest

# Set a version globally (on your ~/.tool-versions file)
asdf global syft latest

# Now syft commands are available
syft version
```

Check [asdf](https://github.com/asdf-vm/asdf) readme for more instructions on how to
install & manage versions.

# Contributing

Contributions of any kind welcome! See the [contributing guide](contributing.md).

[Thanks goes to these contributors](https://github.com/davidgp1701/asdf-syft/graphs/contributors)!

# License

See [LICENSE](LICENSE) © [David Garcia Perez](https://github.com/davidgp1701/)
=======
# asdf-plugin-template [![Build](https://github.com/asdf-vm/asdf-plugin-template/actions/workflows/build.yml/badge.svg)](https://github.com/asdf-vm/asdf-plugin-template/actions/workflows/build.yml) [![Lint](https://github.com/asdf-vm/asdf-plugin-template/actions/workflows/lint.yml/badge.svg)](https://github.com/asdf-vm/asdf-plugin-template/actions/workflows/lint.yml)

This is an [asdf-vm plugin](https://asdf-vm.com/#/plugins-create) template with CI to run [Shellcheck](https://github.com/koalaman/shellcheck) and testing with the [asdf test GitHub Action](https://github.com/asdf-vm/actions).
## Usage

1. Create repository based on [this template](https://github.com/asdf-vm/asdf-plugin-template/generate)
2. Clone locally and run `bash setup.bash`.
3. Adapt your code following the `TODO` notes on `lib/utils.bash`.
4. For developing your plugin further, please read [the plugins create section of the docs](https://asdf-vm.com/#/plugins-create).

>A feature of this plugin-template when hosted on GitHub is the use of [release-please](https://github.com/googleapis/release-please), an automated release tool. It leverages [Conventional Commit messages](https://www.conventionalcommits.org/) to determine semver release type, see the [documentation](https://github.com/googleapis/release-please).

## Contributing

Contributions welcome!

1. Install `asdf` tools
    ```shell
    asdf plugin add shellcheck https://github.com/luizm/asdf-shellcheck.git
    asdf plugin add shfmt https://github.com/luizm/asdf-shfmt.git
    asdf install
    ```
2. Develop!
3. Lint & Format
    ```shell
    ./scripts/shellcheck.bash
    ./scripts/shfmt.bash
    ```
4. PR changes
