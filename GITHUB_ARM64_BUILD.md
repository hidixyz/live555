# GitHub ARM64 Build

This repository includes a GitHub Actions workflow that builds the project in a **Debian 12 (bookworm) ARM64** environment and uploads key executables as an artifact.

## Workflow file

- `.github/workflows/build-arm64.yml` (uses `debian:12-slim` container + `./genMakefiles linux-no-openssl`)

## How to run

1. Push your branch to GitHub.
2. Open **Actions** in your GitHub repository.
3. Run **Build ARM64 Executables** (or push/PR to trigger automatically).
4. Download artifact: **live555-arm64-executables**.

## Build environment details

- Base image: Debian 12 (bookworm)
- glibc: 2.36 series
- Build mode: `linux-no-openssl` (TLS features disabled: RTSPS/SRTP)

## Included executables

- `testRTSPClient`
- `openRTSP`
- `live555ProxyServer`
- `live555MediaServer`
- `live555HLSProxy`
