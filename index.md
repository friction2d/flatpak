# Friction Flatpak Repository

This is the official Flatpak repository for **Friction**. This repository provides both stable releases and nightly builds directly from the source.

## Installation

The easiest way to install Friction is by using the `.flatpakref` files. Most Linux distributions will open these automatically with your software manager (GNOME Software, KDE Discover, etc.).

* [**Install Stable**](https://flatpak.friction.graphics/friction-stable.flatpakref) (Recommended for most users)
* [**Install Nightly**](https://flatpak.friction.graphics/friction-nightly.flatpakref) (Cutting-edge features, potentially unstable)

## Advanced

If you prefer the command line, follow these steps to add the repository and install the application.

```bash
flatpak remote-add --if-not-exists friction-repo https://flatpak.friction.graphics/friction.flatpakrepo
```

### Stable

```bash
flatpak install friction-repo graphics.friction.Friction
```

### Nightly

```bash
flatpak install friction-repo graphics.friction.Friction//nightly
```
