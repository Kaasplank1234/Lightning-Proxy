# ⚡ Lightning Proxy

Lightning Proxy is a desktop proxy client for **macOS, Windows, and Linux**. Import a VLESS REALITY profile or a compatible HTTPS subscription, choose how to route your traffic, and connect. Imported profiles are saved locally and available the next time you open the app.

[Download Lightning Proxy](https://lightning-proxy.pages.dev/#downloads) · [Installation guide](https://lightning-proxy.pages.dev/#installation) · [GitHub release and setup instructions](https://github.com/Kaasplank1234/Lightning-Proxy/releases/tag/Download)

## Technical specifications

| Specification | Details |
| --- | --- |
| Supported protocol | VLESS REALITY over TCP |
| Profile import | `vless://` links and compatible HTTPS subscription URLs |
| Profile storage | Imported profiles are stored locally |
| Device-wide routing | TUN routes TCP and UDP traffic, including traffic from apps without their own proxy settings |
| Local SOCKS5 proxy | `127.0.0.1:10808` |
| Local HTTP proxy | `127.0.0.1:10809` |
| System Proxy | macOS only. Restores the previous system proxy settings when you disconnect |

You’ll need a compatible profile or subscription from your proxy provider to connect.

## Supported platforms

| Platform | Architecture | Download format | Connection modes |
| --- | --- | --- | --- |
| macOS 11 or later | Apple Silicon (ARM64) | DMG | TUN, Local Proxy, System Proxy |
| macOS 11 or later | Intel (x64) | DMG | TUN, Local Proxy, System Proxy |
| Windows 10 or 11 | x64 | ZIP | TUN, Local Proxy |
| Linux | x64 | Flatpak | Local Proxy |
| Linux | x64 | TAR.GZ | TUN, Local Proxy |

On Linux, the **Flatpak** adds Lightning Proxy to your app menu and can fetch the required GNOME runtime on first install. Choose the **TAR.GZ** build for device-wide TUN. That build uses GTK 3 and WebKitGTK, and its TUN setup requires administrator approval and access to `/dev/net/tun`.

## Choose a connection mode

- **TUN** routes traffic device-wide, including traffic from desktop apps that have no proxy settings.
- **Local Proxy** routes traffic from apps you configure to use the local SOCKS5 or HTTP proxy.
- **System Proxy** applies proxy settings on macOS for apps that follow those settings.

## Installation and help

- **macOS** — Choose the DMG for your Mac, install the app, and check the first-launch steps if macOS blocks it.
- **Windows** — Extract the ZIP. If it contains `Lightning Proxy Setup.exe`, run the installer and open Lightning Proxy from the Start menu. If it contains the portable build, run `Lightning Proxy.exe` from the extracted folder.
- **Linux** — Follow the Flatpak steps for Local Proxy or the TAR.GZ steps for TUN. The website includes copyable commands for installing dependencies, downloading the package, launching the app, and setting up TUN.

[Open the installation guide](https://lightning-proxy.pages.dev/#installation) · [Read the GitHub release instructions](https://github.com/Kaasplank1234/Lightning-Proxy/releases/tag/Download)

## Report a problem

Include your operating system, app version, connection mode, and exact error message. Remove subscription URLs, full VLESS links, and credentials before sharing logs or screenshots.

[Open a GitHub issue](https://github.com/Kaasplank1234/Lightning-Proxy/issues)

Made by [Cheesy Studios](https://www.cheesy-studios.22web.org/).
