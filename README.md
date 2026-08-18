# homebrew-ac3forge

A [Homebrew](https://brew.sh) tap for [`ac3cli`](https://github.com/iainchesworthlabs/ac3forge),
the command-line front end for ac3forge — a clean-room AC-3 (ATSC A/52) / E-AC-3 encoder and
decoder with a spatial (Dolby Atmos-style) object layer, in C++23.

## Install

```bash
brew install iainchesworthlabs/ac3forge/ac3forge
```

This builds `ac3cli` from source. The Qt6 GUI (`ac3gui`) is not packaged here — see
[ac3forge's own releases](https://github.com/iainchesworthlabs/ac3forge/releases) for a prebuilt
desktop archive that includes it, or [docs/releasing.md](https://github.com/iainchesworthlabs/ac3forge/blob/main/docs/releasing.md#homebrew-formula)
for why.

## Updating

The formula here is generated from
[`packaging/homebrew/Formula/ac3forge.rb`](https://github.com/iainchesworthlabs/ac3forge/tree/main/packaging/homebrew)
in the main repository, which is kept in sync with each release — see that repository's
`docs/releasing.md` for the update flow. Changes belong there first, then get copied into this
tap.
