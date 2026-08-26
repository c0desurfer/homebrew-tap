# Swift Salamander, on Homebrew

A dual-pane file manager for macOS. Local folders, network shares and 38
storage providers in one native window, written in Rust.

Apple silicon, macOS 13 Ventura or newer.

## Install

```sh
brew install --cask c0desurfer/tap/swift-salamander
```

That is the whole thing. Homebrew adds the tap on first use, downloads the
signed and notarized disk image from the project's own CDN, checks it against
the hash in the cask, and puts `Swift Salamander.app` in `/Applications`.

## Updates

The app updates itself and tells you when a new version is ready, so Homebrew
stays out of the way. `brew upgrade` will not touch it. If you would rather
Homebrew did the work:

```sh
brew upgrade --cask --greedy swift-salamander
```

## Uninstall

```sh
brew uninstall --cask swift-salamander
```

That removes the app and leaves your settings, favourites and licence where
they are, so reinstalling picks up where you left off.

To remove everything, including your licence file:

```sh
brew uninstall --cask --zap swift-salamander
```

`--zap` deletes the app's folders under `~/Library`, and your licence lives in
one of them. Keep a copy of your licence key first if you might come back.

## Where this comes from

This repository is a mirror. Nobody edits it by hand: it is generated from the
Swift Salamander source tree and pushed by the release script, so an edit made
here would be overwritten by the next release.

Something wrong with the package, or with the app? The feedback board is at
<https://feedback.codesurfer.ch/>.

Homepage: <https://salamander.codesurfer.ch/>
