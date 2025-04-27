# A Flatpak App for testing
## Building
> **_NOTE:_**  With io.github.Sdk installed.
```console
flatpak run org.flatpak.Builder build-dir --repo=../repo --force-clean io.github.App.yml
```
---
## Installing Locally
> **_NOTE:_**  From the directory above this
```console
flatpak install --user ./repo io.github.App
```
---
## Removing
```console
flatpak remove io.github.App
```
