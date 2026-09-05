# App4

App4 is a meta-model platform for building software: you describe an
application's backend, web and mobile surfaces in the App4 DSL, and
App4's runtimes execute those models directly. Plugins add
infrastructure (databases, queues, auth, payments, AI) through a common
gRPC contract, and App4 Studio drives the whole loop with AI workers.

This repository is the entry point to the App4 tooling. The documentation
lives at [app4.dev](https://app4.dev).

## Install

**Homebrew** (macOS and Linux; Homebrew 6 asks you to trust a third-party tap once):

```sh
brew tap app4-ai/tap && brew trust app4-ai/tap
brew install --cask app4-studio    # Studio desktop app + the `app4` command (macOS)
brew install app4-cli              # the `app4` command only (macOS and Linux)
```

**npm**:

```sh
npx @app4/cli --version            # run without installing
npm install -g @app4/cli           # or install the `app4` command globally
```

**Shell script** (no package manager required):

```sh
curl -fsSL https://app4.dev/install.sh | sh
```

The script installs the `app4` command into `~/.app4/bin`. Verify with:

```sh
app4 --version
```

## Repositories

| Repository | Purpose |
|------------|---------|
| [homebrew-tap](https://github.com/app4-ai/homebrew-tap) | Homebrew formulae and casks |
| app4-cli | The `app4` command (source moves here at launch) |
| app4-studio | App4 Studio desktop application (source moves here at launch) |

## License

[Apache License 2.0](LICENSE)
