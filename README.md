<p align="center">
  <img src="assets/logo.png" alt="BMBridge Lite" width="240"/>
</p>

<h1 align="center">BMBridge Lite</h1>

<p align="center">
  <b>Custom Notes Bridge for Bookmap</b><br/>
  Serve manual price notes to Bookmap Cloud Notes over local HTTP.
</p>

<p align="center">
  <a href="https://sdes.dev"><img src="https://img.shields.io/badge/publisher-SDES.DEV-d4af37?style=flat-square" alt="SDES.DEV"/></a>
  <img src="https://img.shields.io/badge/platform-Windows-0078d4?style=flat-square" alt="Windows"/>
  <img src="https://img.shields.io/badge/version-Lite%201.0.1-3b82f6?style=flat-square" alt="Version"/>
  <img src="https://img.shields.io/badge/license-Proprietary-ef4444?style=flat-square" alt="License"/>
</p>

---

## Overview

BMBridge Lite is a lightweight Windows application that lets you author custom price notes, render them to CSV in Bookmap's Cloud Notes format, and serve those CSVs on `127.0.0.1` over HTTP so Bookmap can poll and render them as chart annotations.

All notes are user-entered. The program does not source, import, or redistribute market data.

## Features

- Up to **2 concurrent feeds**, each on its own local HTTP port
- **Custom notes** with description, strict-decimal price, text/background colors, alignment, and optional horizontal price line
- **Color templates** — save and reuse color/text combinations. Templates are grouped into Colors-only and Colors+Text sections; names can be reused across sections
- **Sort, reorder, clone, enable/disable** notes per feed
- **Delete feeds** from the tab header — one feed minimum enforced
- **Symbol override** per feed, or shared global symbol
- **Live polling monitor** — per-feed *Last polled* timestamp plus tray-balloon toast if Bookmap stops polling for 2 minutes
- **Runtime Broadcasting toggle** — start or stop a feed's server on demand while the app is live
- **UI font size** — five presets, applies instantly
- **System tray integration** — minimize to tray and keep servers running in the background
- **Single-instance** enforcement — only one copy can run at a time
- **Atomic settings writes, UTF-8 safe** — your notes and templates are preserved across sessions
- **Tooltips everywhere** — hover any control for a short explanation

## Download

Get the latest release from the [**Releases**](../../releases) page.

Each release ships as a zip containing:

```
BMBridge_Lite.exe
BMBridgeLite.ico
BMBridge_Lite_Quick_Start.pdf
BMBridge_Lite_User_Manual.pdf
README.txt
(Nuitka-bundled Python runtime and DLLs)
```

## Installation

1. Download the latest `BMBridge_Lite_vLite-1.0.zip` from Releases.
2. Unzip to any folder with write access.
3. Run `BMBridge_Lite.exe`.
4. On first launch, Windows SmartScreen may show "Windows protected your PC" because the EXE is not code-signed. Click **More info** -> **Run anyway**.
5. Read and accept the first-run disclaimer.
6. Follow the Quick-Start guide.

## Documentation

- [Quick-Start Guide](docs/BMBridge_Lite_Quick_Start.pdf) - get your first note on a Bookmap chart in under five minutes
- [User Manual](docs/BMBridge_Lite_User_Manual.pdf) - full reference, settings, troubleshooting
- [Bookmap Cloud Notes reference](https://bookmap.com/knowledgebase/docs/KB-Appendices-AII-CustomNotes) - authoritative Bookmap-side setup

## Known Issues

As of 1.0.1, no material known issues.

Note that sort and delete operations have no undo — back up `bridge_lite_settings.json` before large reorganizations.

## Disclaimer

BMBridge Lite is an independent, third-party software application developed by SDE-Software (SDES.DEV). It is **not affiliated with, endorsed by, sponsored by, or in any way connected to Bookmap**, or any of its parent companies, subsidiaries, licensors, or affiliated entities. Bookmap is a trademark of Bookmap Ltd.

BMBridge Lite is provided **as-is** and is **used entirely at the user's own risk**. The developer accepts no liability for incorrect note content, file corruption, server failures, Bookmap rendering behavior, or any trading decisions made based on notes displayed by this application.

**No support, walkthroughs, troubleshooting, or individual assistance is provided by SDES.DEV, Bookmap, Tom B, the Bookmap Discord channels, or the Bookmap support team.** Users are responsible for reading the included documentation and the official Bookmap Cloud Notes reference.

Bugs and glitches are addressed as identified. No service-level agreement is offered.

## License

Proprietary - see [LICENSE](LICENSE). The binaries distributed here may be downloaded and used, but may not be redistributed, resold, modified, reverse-engineered, or repackaged without prior written permission from SDE-Software (SDES.DEV).

## Publisher

[SDES.DEV](https://sdes.dev) - SDE-Software
