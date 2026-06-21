# Subcor Homebrew Tap

Homebrew tap for the [Subcor](https://subcor.ai) CLI on macOS.

## Install

```sh
brew install subcor-ai/tap/subcor
```

Or in two steps:

```sh
brew tap subcor-ai/tap
brew install subcor
```

Upgrade with `brew upgrade subcor`; remove with `brew uninstall subcor`.

Homebrew installs are macOS only. On Linux, use the installer at
<https://get.subcor.ai>.

## What's here

- `Casks/subcor.rb` — the cask for the Subcor CLI. **Machine-generated** on each
  release by the Subcor build pipeline (GoReleaser); do **not** hand-edit it —
  changes are overwritten on the next release.

The CLI binaries are compiled from a private source repository and published to
<https://get.subcor.ai>; this tap's cask points at those same release assets, so
`brew install` gives you the identical binary the `curl … | sh` installer does.
