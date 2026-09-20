# Valkor CLI

This is the public distribution repository for the Valkor command-line
client. The CLI source remains in a private repository; this repository only
contains the installer, release metadata, and prebuilt binaries attached to
GitHub Releases.

## Install

```sh
curl -fsSL https://beeuni.ai/install | bash
```

The installer detects macOS or Linux and downloads the matching binary for
`arm64` or `x64` from the latest stable release in this repository.

To install a specific version:

```sh
curl -fsSL https://beeuni.ai/install | VALKOR_VERSION=0.1.3 bash
```

The release assets are named:

```text
valkor-darwin-arm64
valkor-darwin-x64
valkor-linux-arm64
valkor-linux-x64
SHA256SUMS
```

## Usage

```sh
valkor login
valkor projects ls
valkor projects link
valkor --help
```

The CLI connects to the Valkor platform API at `https://valkorapi.beeuni.ai` by default.
Use `valkor login --help` to configure a different host or API endpoint.

## Releases

Releases are built from the private Valkor source repository and published
here by the release workflow. This repository does not contain the CLI source
code or the private platform configuration.
