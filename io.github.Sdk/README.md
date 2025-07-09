# A Flatpak SDK for testing
## Building
> **_NOTE:_**  With org.freedesktop.Sdk and org.freedesktop.Platform installed.
```console
flatpak run org.flatpak.Builder build-dir --repo=../repo --force-clean io.github.Sdk.yml
```
## Installing
### Locally
```console
flatpak install --user ../repo io.github.Sdk io.github.Platform
```
### Remote
> **_NOTE:_**  With https://chrishobday.github.io/FlatpakTesting/repo.flatpakrepo added
```console
flatpak install io.github.Sdk io.github.Platform
```
## Removing
```console
flatpak remove io.github.Sdk io.github.Platform
```
