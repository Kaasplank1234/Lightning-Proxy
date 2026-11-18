# ⚡ Lightning Proxy

Lightning Proxy is a desktop proxy client for macOS, Windows, and Linux. Import a VLESS REALITY profile or a compatible HTTPS subscription, choose a connection mode, and connect. Profiles are saved locally so they’re available the next time you open the app.

[View releases on GitHub](https://github.com/Kaasplank1234/Lightning-Proxy/releases)

## Downloads

| Platform | Package |
| --- | --- |
| macOS 11 or later · Apple Silicon | `Lightning-Proxy-5.2-macOS-AppleSilicon.dmg` |
| macOS 11 or later · Intel | `Lightning-Proxy-5.2-macOS-Intel.dmg` |
| Windows 10 or 11 · x64 | `Lightning-Proxy-5.2-Windows-x64.zip` |
| Linux · x64 | `Lightning-Proxy-5.2-Linux-x64.tar.gz` |

You’ll need a VLESS profile or compatible subscription from your proxy provider to connect.

## Installation

- **macOS** — Open the DMG for your processor and drag **Lightning Proxy** into **Applications**. macOS may show a Gatekeeper prompt because the build isn’t Apple-notarized. The first time you enable a system mode, the app may ask for administrator approval to install its networking helpers.
- **Windows** — Extract the entire ZIP and run **Lightning Proxy.exe** from the extracted folder. TUN mode may trigger a Windows administrator prompt.
- **Linux** — Extract the archive, install GTK 3 and WebKitGTK if needed, and run `./lightning-proxy` from the extracted directory. To enable TUN, run `./Setup-Tunnel.sh` once. TUN requires `/dev/net/tun`.

## Connection modes

| Mode | How it routes traffic |
| --- | --- |
| TUN | Routes TCP and UDP traffic device-wide, including traffic from apps without proxy settings. |
| Local Proxy | Lets you configure individual apps to use SOCKS5 at `127.0.0.1:10808` or HTTP at `127.0.0.1:10809`. |
| System Proxy · macOS | Sets the macOS proxy for apps that respect system settings and restores the previous settings on disconnect. |

## First connection

1. Import a `vless://` link or a compatible HTTPS subscription URL.
2. Select the imported profile.
3. Choose **TUN** for device-wide routing or **Local Proxy** to configure apps individually.
4. Connect and check the status in Lightning Proxy.

If a connection fails, try a freshly imported profile. If Local Proxy connects but TUN doesn’t, check whether the app received permission to configure the tunnel.

## Feedback

Report problems through [GitHub Issues](https://github.com/Kaasplank1234/Lightning-Proxy/issues). Include your operating system, app version, connection mode, and the error message. Keep subscription URLs and full VLESS links private because they can contain credentials.

Made by [Cheesy Studios](https://www.cheesy-studios.22web.org/).
