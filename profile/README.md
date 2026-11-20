<p align="center">
  <img src="https://raw.githubusercontent.com/helixdesktop/.github/main/brand/helix-x-cover.png" alt="Helix: a fresh desktop for Linux, with everything you already use." width="100%">
</p>

# Helix

**Helix** is a Wayland desktop environment written in Rust. It starts out compatible with GNOME's public contracts (D-Bus interfaces, GSettings schemas, portals and Wayland protocols) and is designed to grow beyond them.

Existing GTK, libadwaita, Qt, Chromium/Electron and X11 applications run unchanged, next to the GNOME services they expect. Helix is a clean-room implementation, not a fork of GNOME, and it is already in daily use as a primary desktop.

🌐 [helixdesktop.org](https://helixdesktop.org)

## Repositories

| Repository | What it holds |
|---|---|
| [**desktop**](https://github.com/helixdesktop/desktop) | The desktop itself: the `helix-comp` compositor (Smithay, DRM/KMS, Xwayland), the `helix-shell` shell, the `helix-session` session manager, xdg-desktop-portal backends and the optional `helix-greeter` login screen |
| [**apps**](https://github.com/helixdesktop/apps) | Helix's own applications, a drop-in replacement for the GNOME core apps (Files, Settings, Terminal, Text Editor and more) |
| [**spec**](https://github.com/helixdesktop/spec) | The living specification: the contracts Helix implements, and the choices it makes wherever GNOME's behaviour is undocumented |
| [**web**](https://github.com/helixdesktop/web) | The source for [helixdesktop.org](https://helixdesktop.org) and its documentation |

## Getting started

Download the `.deb` packages from the [desktop releases](https://github.com/helixdesktop/desktop/releases) and the [apps releases](https://github.com/helixdesktop/apps/releases). Install them together, then choose the **Helix** session at the login screen. The [desktop README](https://github.com/helixdesktop/desktop#installing-and-using-helix) has the full steps.

## Contributing

New features are written up in [spec](https://github.com/helixdesktop/spec) first and implemented afterwards. Report bugs in the repository the problem is in.

AI-assisted contributions are welcome, held to the same standards as any other: you are responsible for what you submit, test it, and say that a tool helped. See [CONTRIBUTING.md](https://github.com/helixdesktop/.github/blob/main/CONTRIBUTING.md).

All Helix code and documentation is released under [CC0-1.0](https://creativecommons.org/publicdomain/zero/1.0/).
