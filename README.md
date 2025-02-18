# Testing
## Installing
- Download com.github.Testing.flatpak from releases
- Install com.github.Testing.flatpak (sudo needed for installing single use Flatpak bundle)
```console
sudo flatpak install com.github.Testing.flatpak
```
## Launching
- Launch the Testing Flatpak (Either search for the app in your menu and click it) or
```console
flatpak run com.github.Testing
```
## Uninstalling
- Remove Testing Flatpak
```console
flatpak remove com.github.Testing
```
## Downloading/Cloning this repo
- Click the green button to download zip and extract once downloaded or clone repo with
```console
git clone --recurse-submodules https://github.com/ChrisHobday/com.github.Testing
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
- Build the Flatpak with flatpak-builder (Run this from within the com.github.Testing directory)
```console
flatpak run org.flatpak.Builder --force-clean --repo=repo build-dir com.github.Testing.yml
```
## User installation while building
- Replace last Building step with
```console
flatpak run org.flatpak.Builder --force-clean --repo=repo --user --install build-dir com.github.Testing.yml
```
## Building single use Flatpak bundle like in the releases (After having followed the Building steps above)
- Build the Flatpak bundle (Run this from within the com.github.Testing directory after having followed the Building steps above)
```console
flatpak build-bundle repo com.github.Testing.flatpak com.github.Testing
```
## Troubleshooting
- Check if Flatpak is installed
```console
flatpak list | grep Testing
```
- Enter Flatpak in command line mode
```console
flatpak run --command=sh com.github.Testing
```
## Flatpak locations
- Installation directory             = /var/lib/flatpak/app/com.github.Testing/
- Installation directory (User mode) = ~/.local/share/flatpak/app/com.github.Testing/
- User cache directory               = ~/.var/app/com.github.Testing/cache/
- User config directory              = ~/.var/app/com.github.Testing/config/
- User data directory                = ~/.var/app/com.github.Testing/data/
