protontricks for Flatpak
========================

[protontricks](https://github.com/Matoking/protontricks) compatible with the Flatpak version of Steam.

# Installation

You can install protontricks for Flatpak from the Flathub repository. You need to have Flatpak installed with the Flathub repository configured. For installing Flatpak and configuring Flathub, see the [official installation instructions](https://flatpak.org/setup/).

Install Protontricks for Flatpak using the following command:

```sh
flatpak install flathub com.valvesoftware.Steam.Utility.protontricks
```

Add an alias that allows you to call protontricks using the `protontricks-flat` alias:

```sh
echo "alias protontricks-flat='flatpak run --command=protontricks com.valvesoftware.Steam --no-runtime'" >> ~/.bashrc
```

**You will need to restart any terminal emulators you have open for the alias to take effect.**

# Usage

After you have installed Protontricks and added the alias, you can use Protontricks with the Flatpak version of Steam using the alias you configured:

```sh
# Note that you need to call `protontricks-flat` instead of `protontricks`

# Find your game's App ID by searching for it
protontricks-flat -s <GAME NAME>

# Run winetricks for the game
protontricks-flat <APPID> <ACTIONS>
```

For the rest of the usage options, [see the README](https://github.com/Matoking/protontricks/blob/master/README.md) on the main Protontricks repository.
