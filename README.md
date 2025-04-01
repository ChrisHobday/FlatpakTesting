# Flatpak Testing
## Building
```console
flatpak-builder build-dir --repo=repo --force-clean io.github.App.yml
```

> **_NOTE:_**  With io.github.App installed.
```console
flatpak-builder build-dir --repo=repo --force-clean io.github.App.extensions.extension.yml
```

> **_NOTE:_**  With io.github.App installed.
```console
flatpak-builder build-dir --repo=repo --force-clean io.github.App.BaseExtender.yml
```

```console
flatpak-builder build-dir --repo=repo --ccache --force-clean org.wine.Sdk.yml
```

> **_NOTE:_**  With org.wine.Sdk and org.wine.Platform installed.
```console
flatpak-builder build-dir --repo=repo --force-clean org.wine.App.yml
```
