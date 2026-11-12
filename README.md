# Idyl Labs Homebrew tap

Homebrew casks for Idyl Labs command-line tools, for macOS and Linux on
amd64 and arm64. Homebrew picks the build for the machine it runs on.

| Cask | Installs |
| --- | --- |
| `idyl` | `idyl`, the command-line client for IDYL, with its bash, zsh and fish completion scripts |
| `purlview` | `purlview`, which shares a running app for live feedback, with its manual pages and bash, zsh and fish completion scripts |

## idyl

```sh
brew install --cask idyl-labs/tap/idyl
brew upgrade --cask idyl
brew uninstall --cask idyl
```

The cask downloads each release from IDYL's download site, `get.idyl.sh`.

## purlview

```sh
brew install --cask idyl-labs/tap/purlview
brew upgrade --cask purlview
brew uninstall --cask purlview
```

Upgrading or uninstalling Purlview stops its local daemon and ends any
active shares; start a share again afterwards.

## How the casks are published

Each project's release workflow writes its cask for every stable release and
commits it here, so a change made directly to a cask is replaced by the next
release. Prereleases are not published to the tap.
