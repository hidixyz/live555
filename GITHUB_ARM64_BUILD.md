# GitHub ARM64 Build

This repository includes a GitHub Actions workflow that builds the project on an ARM64 runner without OpenSSL/TLS dependencies and uploads key executables as an artifact.

## Workflow file

- `.github/workflows/build-arm64.yml` (uses `./genMakefiles linux-no-openssl`)

## How to run

1. Push your branch to GitHub.
2. Open **Actions** in your GitHub repository.
3. Run **Build ARM64 Executables** (or push/PR to trigger automatically).
4. Download artifact: **live555-arm64-executables**.

## Notes for Debian 11 ARM64 (no OpenSSL 3)

- The workflow intentionally uses `linux-no-openssl` so it does not require OpenSSL 3.
- TLS-related functionality (RTSPS/SRTP) is disabled in this build.

## Included executables

- `testRTSPClient`
- `openRTSP`
- `live555ProxyServer`
- `live555MediaServer`
- `live555HLSProxy`
