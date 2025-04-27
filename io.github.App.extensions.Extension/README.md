# A Flatpak App Extension for testing
> **_NOTE:_**  With io.github.App installed.
## Building
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
