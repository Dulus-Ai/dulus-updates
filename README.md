# Dulus Premium updates

This repository is the public release channel for Dulus Premium desktop
artifacts. It contains release binaries and their SHA-256 sidecars only; the
Premium source code and customer data stay private.

## Release contract

- Tags use `vX.Y.Z` (for example `v3.12.0`).
- Windows: `Dulus-X.Y.Z-windows-setup.exe`
- macOS Apple Silicon: `Dulus-X.Y.Z-macos-arm64.dmg`
- macOS Intel: `Dulus-X.Y.Z-macos-x86_64.dmg`
- Linux: `Dulus-X.Y.Z-linux.AppImage`
- Each installer should ship with a matching `<asset>.sha256` sidecar.

Premium checks this channel once at startup and then once every 24 hours while
the app is open. Updates are announced non-blockingly; the user opens the
GitHub release page and installs the signed artifact manually.
