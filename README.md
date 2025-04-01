# Flatpak Testing
## Building
```console
flatpak-builder build-dir --repo=repo --force-clean io.github.App.yml
```
---
> **_NOTE:_**  With io.github.App installed.
```console
flatpak-builder build-dir --repo=repo --force-clean io.github.App.extensions.Extension.yml
```
---
> **_NOTE:_**  With io.github.App installed.
```console
flatpak-builder build-dir --repo=repo --force-clean io.github.App.BaseExtender.yml
```
---
```console
flatpak-builder build-dir --repo=repo --ccache --force-clean org.wine.Sdk.yml
```
---
> **_NOTE:_**  With org.wine.Sdk and org.wine.Platform installed.
```console
flatpak-builder build-dir --repo=repo --force-clean org.wine.App.yml
```
## Adding repo
```console
flatpak remote-add --if-not-exists repo https://chrishobday.github.io/FlatpakTesting/repo.flatpakrepo
```
## Installing from repo
```console
flatpak install io.github.App
```
---
```console
flatpak install io.github.App.extensions.Extension
```
---
```console
flatpak install io.github.App.BaseExtender
```
---
```console
flatpak install org.wine.App
```