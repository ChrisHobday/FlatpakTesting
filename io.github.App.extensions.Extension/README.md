# A Flatpak App Extension for testing
## Building
> **_NOTE:_**  With io.github.Sdk and io.github.App installed.
```console
flatpak run org.flatpak.Builder build-dir --repo=../repo --force-clean io.github.App.extensions.Extension.yml
```
---
## Installing
> **_NOTE:_**  From the directory above this
```console
flatpak install --user ./repo io.github.App.extensions.Extension
```
---
## Removing
```console
flatpak remove io.github.App.extensions.Extension
```
