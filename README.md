# ⚡ Lightning Proxy

Lightning Proxy is a desktop proxy client for **macOS, Windows, and Linux**. Import a VLESS REALITY profile or a compatible HTTPS subscription, choose how to route your traffic, and connect. Imported profiles are saved locally and available the next time you open the app.

[Download Lightning Proxy](https://lightning-proxy.pages.dev/#downloads) · [Installation guide](https://lightning-proxy.pages.dev/#installation) · [GitHub Releases](https://github.com/Kaasplank1234/Lightning-Proxy/releases)

## Technical specifications

| Specification | Details |
| --- | --- |
| Supported protocol | VLESS REALITY over TCP |
| Profile import | `vless://` links and compatible HTTPS subscription URLs |
| Profile storage | Imported profiles are stored locally |
| Device-wide routing | TUN mode routes TCP and UDP traffic, including traffic from apps without their own proxy settings |
| Local SOCKS5 proxy | `127.0.0.1:10808` |
| Local HTTP proxy | `127.0.0.1:10809` |
| System Proxy | macOS only. Restores the previous system proxy settings when you disconnect |

Lightning Proxy uses a profile or subscription supplied by your proxy provider. You’ll need one to connect.

## Supported platforms

| Platform | Architecture | Download format |
| --- | --- | --- |
| macOS 11 or later | Apple Silicon (ARM64) | DMG |
| macOS 11 or later | Intel (x64) | DMG |
| Windows 10 or 11 | x64 | ZIP |
| Linux | x64 | TAR.GZ |

The Linux app uses GTK 3 and WebKitGTK. Linux TUN mode also requires `/dev/net/tun`. Enabling TUN for the first time may require administrator approval.

## Choose a connection mode

- **TUN** routes traffic device-wide. Use it for desktop apps that don’t offer their own proxy settings.
- **Local Proxy** routes traffic from apps you configure to use the local SOCKS5 or HTTP proxy.
- **System Proxy** applies proxy settings on macOS for apps that follow those settings.

## Installation and help

See the [Lightning Proxy installation guide](https://lightning-proxy.pages.dev/#installation) for setup on macOS, Windows, and Linux, including how to open the app on macOS and enable TUN. The website also covers your first connection and common connection problems.

## Report a problem

Open an issue on [GitHub](https://github.com/Kaasplank1234/Lightning-Proxy/issues). Include your operating system, app version, connection mode, and exact error message. Remove subscription URLs, full VLESS links, and credentials before sharing logs or screenshots.

Made by [Cheesy Studios](https://www.cheesy-studios.22web.org/).
