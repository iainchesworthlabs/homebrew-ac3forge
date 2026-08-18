# homebrew-ac3forge

A [Homebrew](https://brew.sh) tap for [ac3forge](https://github.com/iainchesworthlabs/ac3forge) —
a clean-room AC-3 (ATSC A/52) / E-AC-3 encoder and decoder with a spatial (Dolby Atmos-style)
object layer, in C++23. Two independent packages: `ac3forge` (the `ac3cli` command-line front
end, a Formula built from source) and `ac3gui` (the Qt6 GUI, a Cask installing the prebuilt
`.app` from a release's `.dmg`) — install either, both, or neither.

## Install

```bash
brew install iainchesworthlabs/ac3forge/ac3forge
```

Builds `ac3cli` from source.

```bash
brew install --cask iainchesworthlabs/ac3forge/ac3gui
```

Installs the prebuilt `ac3gui.app` (Apple Silicon only, macOS Ventura or later). It is not
Apple-notarized or code-signed — expect a Gatekeeper "developer cannot be verified" prompt on
first launch; see the Cask's own `caveats` (`brew info --cask ac3gui`) for the one-line
workaround.

## Updating

Both files here are generated from the main repository —
[`packaging/homebrew/Formula/ac3forge.rb`](https://github.com/iainchesworthlabs/ac3forge/tree/main/packaging/homebrew/Formula)
and
[`packaging/homebrew/Casks/ac3gui.rb`](https://github.com/iainchesworthlabs/ac3forge/tree/main/packaging/homebrew/Casks) —
which are kept in sync with each release; see that repository's
[`docs/releasing.md`](https://github.com/iainchesworthlabs/ac3forge/blob/main/docs/releasing.md#homebrew-formula-and-cask)
for the update flow. Changes belong there first, then get copied into this tap.
