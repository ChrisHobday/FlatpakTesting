# Testing
## Installing
- Download flatpak.test.app.flatpak from releases
- Install flatpak.test.app.flatpak (sudo needed for installing single use Flatpak bundle)
```console
sudo flatpak install flatpak.test.app.flatpak
```
```console
sudo flatpak install flatpak.test.app.extension.test.flatpak
```
## Launching
- Launch the Testing Flatpak (Either search for the app in your menu and click it) or
```console
flatpak run flatpak.test.app
```
## Uninstalling
- Remove Testing Flatpak
```console
flatpak remove flatpak.test.app
```
```console
flatpak remove flatpak.test.app.extension.test
```
## Downloading/Cloning this repo
- Click the green button to download zip and extract once downloaded or clone repo with
```console
git clone --recurse-submodules https://github.com/ChrisHobday/flatpak.test.app
```
## Building
- Install Flatpak builder
```console
flatpak install flathub org.flatpak.Builder
```
- Install the platform this Flatpak will be using
```console
flatpak install flathub org.freedesktop.Platform//24.08 org.freedesktop.Sdk//24.08
```
- Build the Flatpak and Extension with flatpak-builder (Run this from within the flatpak.test.app directory)
```console
flatpak run org.flatpak.Builder --force-clean --repo=repo build-dir flatpak.test.app.yml
```
```console
flatpak run org.flatpak.Builder --force-clean --repo=repo build-dir flatpak.test.app.extension.test.yml
```
## User installation while building
- Replace last Building step with
```console
flatpak run org.flatpak.Builder --force-clean --repo=repo --user --install build-dir flatpak.test.app.yml
```
```console
flatpak run org.flatpak.Builder --force-clean --repo=repo --user --install build-dir flatpak.test.app.extension.test.yml
```
## Building single use Flatpak bundle like in the releases (After having followed the Building steps above)
- Build the Flatpak bundle (Run this from within the flatpak.test.app directory after having followed the Building steps above)
```console
flatpak build-bundle repo flatpak.test.app.flatpak flatpak.test.app
```
```console
flatpak build-bundle --runtime repo flatpak.test.app.extension.test.flatpak flatpak.test.app.extension.test
```
## Troubleshooting
- Check if Flatpak is installed
```console
flatpak list | grep Testing
```
- Enter Flatpak in command line mode
```console
flatpak run --command=sh flatpak.test.app
```
## Flatpak locations
- Installation directory             = /var/lib/flatpak/app/flatpak.test.app/
- Installation directory (User mode) = ~/.local/share/flatpak/app/flatpak.test.app/
- User cache directory               = ~/.var/app/flatpak.test.app/cache/
- User config directory              = ~/.var/app/flatpak.test.app/config/
- User data directory                = ~/.var/app/flatpak.test.app/data/
