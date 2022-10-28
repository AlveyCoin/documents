---
id: installation
title: Installation
---

Please refer to the installation method more applicable to you.

Our recommendation is to use the pre-built releases and verify the provided checksums.

## Pre-built releases

Please refer to the [GitHub Releases](https://github.com/alveychain-lab/alveychain/releases) page for a list of releases.

Alveychain comes with cross-compiled AMD64/ARM64 binaries for Darwin and Linux.

--- 

## Docker image

Official Docker images are hosted under the [hub.docker.com registry](https://hub.docker.com/r/alveychainlab/alveychain).

`docker pull alveychainlab/alveychain:latest`

---

## Building from source

Prior to using `go install` make sure that you have Go `>=1.16` installed and properly configured.

The stable branch is `develop`.

```shell
git clone https://github.com/alveychain-lab/alveychain.git
cd alveychain/
go build main.go -o alveychain
sudo mv alveychain /usr/local/bin
```

---

## Using `go install`

Prior to using `go install` make sure that you have Go `>=1.16` installed and properly configured.

`go install github.com/alveychain-lab/alveychain@dev`

The binary will be available in your `GOBIN` environment variable, and will include the latest changes from the mainline `develop` branch.
