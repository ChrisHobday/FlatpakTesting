# A Flatpak App for testing
## Building
> **_NOTE:_**  With io.github.Sdk and io.github.Platform installed.
```console
flatpak run org.flatpak.Builder build-dir --repo=../repo --force-clean io.github.App.yml
```
## Installing
### Locally
```console
flatpak install --user ../repo io.github.App
```
### Remote
> **_NOTE:_**  With https://chrishobday.github.io/FlatpakTesting/repo.flatpakrepo added
```console
flatpak install io.github.App
```
## Removing
```console
flatpak remove io.github.App
```
## Updating External Data
> **_NOTE:_**  With org.flathub.flatpak-external-data-checker installed.
```console
flatpak run org.flathub.flatpak-external-data-checker --update ./io.github.App.yml
```