# Retinue Launcher

**One place to install, update and launch the PCB engineering tools: CastGuidance PCB Toolkit, FishLadder and EyeOpener Lite.**

> **Releases-only repository.** This repo hosts the prebuilt Windows installer for Retinue Launcher. The source code is proprietary and lives in a private repository.

## Get the latest release

→ **[Download the latest release](https://github.com/otac0011/RetinueLauncher-Releases/releases/latest)** (Windows installer, about 36 MB)

Run `RetinueLauncher-Setup-<version>.exe`. The installer shows the End User License Agreement, which you must accept to install. It installs to `Program Files\Retinue Launcher` (it asks for administrator rights), adds a Start Menu entry and an uninstaller (Settings → Apps). The launcher is self-contained: no separate .NET install is needed.

### Windows SmartScreen

The installer is not code-signed yet, so Windows may show **"Windows protected your PC"** the first time you run it. Click **More info → Run anyway**. You can check the download against the SHA-256 digest shown for the asset on the release page.

### System requirements

- Windows 10 or 11, 64-bit (x64)
- About 130 MB of disk space for the launcher, plus whatever tools you install
- Internet access to list and download tools (installed tools launch offline)

## What it does

The **Available tools** tab lists each tool with its state: *Not installed*, *Installed*, *Update available* or *No release yet*.

| Tool | What it is | Releases |
|---|---|---|
| CastGuidance PCB Toolkit | Around 50 PCB calculators and wizards: impedance, stackups, SI, PI, RF, thermal | [CastGuidance_PCB_Toolkit](https://github.com/otac0011/CastGuidance_PCB_Toolkit) |
| FishLadder | RF impedance matching for people who have never designed a matching network | [FishLadder-Releases](https://github.com/otac0011/FishLadder-Releases) |
| EyeOpener Lite | Guided signal- and power-integrity checks for ODB++ boards | [EyeOpenerLite-Releases](https://github.com/otac0011/EyeOpenerLite-Releases) |

**Nothing is installed until you choose it.** When you press **Install** (or **Update**), the launcher:

1. reads the tool's latest published release from GitHub (anonymously: no account, no token);
2. downloads that release's installer, showing progress, only from the tool's own release page;
3. checks the download's size and its SHA-256 digest against the release, and discards it if either differs;
4. runs the tool's own installer, which shows that tool's license for you to accept.

**Launch** starts an installed tool. The launcher only goes online when you open or refresh the Available tools tab, or press Install.

## License

Distributed under a **proprietary End User License Agreement**; see [`LICENSE`](LICENSE). Open-source components it ships are listed with their licenses in [`THIRD-PARTY-NOTICES.txt`](THIRD-PARTY-NOTICES.txt). Each tool it installs has its own license, shown by that tool's installer.

**Summary** (the file is authoritative):

- ✅ Install and use on any device you own: personal, educational, or commercial
- ✅ Share **unmodified** copies (no fee)
- ❌ Sell, sublicense, or rent
- ❌ Modify, reverse-engineer, or create derivative works
- ❌ Distribute in modified form
- ❌ Remove or obscure copyright notices

This is **not** open-source software. Source code is held privately.

## Reporting a bug

[Open an issue](https://github.com/otac0011/RetinueLauncher-Releases/issues). Please include the launcher version (Settings → Apps, or the file properties of `RetinueLauncher.exe`), what you pressed, and a screenshot if applicable.

---

© 2026 Retinue Launcher Developer. All rights reserved.
