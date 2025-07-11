# A Flatpak Testing repo
## Adding repo
```console
flatpak remote-add --if-not-exists repo https://chrishobday.github.io/FlatpakTesting/repo.flatpakrepo
```
## Installing from repo
```console
flatpak install io.github.Sdk
```
```console
flatpak install io.github.App
```
```console
flatpak install io.github.App.extensions.Extension
```
```console
flatpak install io.github.App.BaseExtender
```
## Removing repo
```console
flatpak remote-delete repo
```
## Updating repo
```console
flatpak build-update-repo --gpg-sign=<gpg-key> --generate-static-deltas --prune repo
```