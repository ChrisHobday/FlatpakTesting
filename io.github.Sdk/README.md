# A Flatpak SDK for testing
## Required Packages
```console
flatpak install org.freedesktop.Sdk//24.08 org.freedesktop.Platform//24.08
```
---
## Building
```console
flatpak run org.flatpak.Builder build-dir --repo=../repo --force-clean io.github.Sdk.yml
```
---
## Installing Locally
> **_NOTE:_**  From the directory above this
```console
flatpak install --user ./repo io.github.Sdk io.github.Platform
```
---
## Removing
```console
flatpak remove io.github.Sdk io.github.Platform
```
