# GitHub ARM64 Build

This repository includes a GitHub Actions workflow that builds the project on an ARM64 runner and uploads key executables as an artifact.

## Workflow file

- `.github/workflows/build-arm64.yml`

## How to run

1. Push your branch to GitHub.
2. Open **Actions** in your GitHub repository.
3. Run **Build ARM64 Executables** (or push/PR to trigger automatically).
4. Download artifact: **live555-arm64-executables**.

## Included executables

- `testRTSPClient`
- `openRTSP`
- `live555ProxyServer`
- `live555MediaServer`
- `live555HLSProxy`
