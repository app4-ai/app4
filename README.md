# App4

App4 is a meta-model platform for building software: you describe an
application's backend, web and mobile surfaces in the App4 DSL, and
App4's runtimes execute those models directly. Plugins add
infrastructure (databases, queues, auth, payments, AI) through a common
gRPC contract, and App4 Studio drives the whole loop with AI workers.

This repository is the entry point to the App4 tooling. The documentation
lives at [app4.dev](https://app4.dev).

## Install

**Homebrew** (macOS and Linux):

```sh
brew install app4-ai/tap/app4-cli              # the `app4` command
brew install --cask app4-ai/tap/app4-studio    # Studio desktop app + CLI
```

**Shell script** (no package manager required):

```sh
curl -fsSL https://app4.dev/install.sh | sh
```

The script installs the `app4` command into `~/.app4/bin`. Verify with:

```sh
app4 --version
```

The first public release through these channels is being prepared.

## Repositories

| Repository | Purpose |
|------------|---------|
| [homebrew-tap](https://github.com/app4-ai/homebrew-tap) | Homebrew formulae and casks |
| app4-cli | The `app4` command |
| app4-studio | App4 Studio desktop application |

## License

[Apache License 2.0](LICENSE)
