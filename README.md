# 🗂️ Nemo Actions

> A collection of actions for the [Nemo](https://github.com/linuxmint/nemo) file manager — Linux Mint / Cinnamon desktop.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/pzim-claude/nemo-actions/blob/main/LICENSE)
[![Stars](https://img.shields.io/github/stars/pzim-claude/nemo-actions?style=flat)](https://github.com/pzim-claude/nemo-actions/stargazers)
[![Last commit](https://img.shields.io/github/last-commit/pzim-claude/nemo-actions)](https://github.com/pzim-claude/nemo-actions/commits/main)
[![Commits](https://img.shields.io/github/commit-activity/t/pzim-claude/nemo-actions)](https://github.com/pzim-claude/nemo-actions/commits/main)
[![Repo size](https://img.shields.io/github/repo-size/pzim-claude/nemo-actions)](https://github.com/pzim-claude/nemo-actions)
[![Visitors](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Fpzim-claude%2Fnemo-actions&count_bg=%2379C83D&title_bg=%23555555&icon=github.svg&icon_color=%23E7E7E7&title=visitors&edge_flat=false)](https://hits.seeyoufarm.com)

---

## ⚡ Quick Install

Download the `.zip` of any action and extract it to `~/.local/share/nemo/actions/`:

```bash
unzip action@pzim-devdata.zip -d ~/.local/share/nemo/actions && nemo -q
```

Or use the **one-line install** command from each action's page.

---

## 📦 Actions

| Action | Description | Downloads | Install |
|--------|-------------|-----------|---------|
| [🖨️ Convert to PDF](#️-convert-to-pdf) | Convert documents and images to PDF | [![Downloads](https://img.shields.io/github/downloads/pzim-claude/nemo-actions/latest/convert-to-pdf@pzim-devdata.zip)](https://github.com/pzim-claude/nemo-actions/releases/latest) | [README](convert-to-pdf@pzim-devdata/README.md) |
| [😀 Copy an Emoticon](#-copy-an-emoticon) | Quick access to emoticons with clipboard copy | [![Downloads](https://img.shields.io/github/downloads/pzim-claude/nemo-actions/latest/copy-emoticon@pzim-devdata.zip)](https://github.com/pzim-claude/nemo-actions/releases/latest) | [README](copy-emoticon@pzim-devdata/README.md) |
| [🔒 Hidden Actions](#-hidden-actions) | Execute scripts via Ctrl+Right-click | [![Downloads](https://img.shields.io/github/downloads/pzim-claude/nemo-actions/latest/hidden-actions@pzim-devdata.zip)](https://github.com/pzim-claude/nemo-actions/releases/latest) | [README](hidden-actions@pzim-devdata/README.md) |
| [📥 Install Debian Package](#-install-debian-package) | Install .deb with auto dependency resolution | [![Downloads](https://img.shields.io/github/downloads/pzim-claude/nemo-actions/latest/install-deb-package@pzim-devdata.zip)](https://github.com/pzim-claude/nemo-actions/releases/latest) | [README](install-deb-package@pzim-devdata/README.md) |
| [🎬 Display Media Information](#-display-media-information) | Detailed media info via MediaInfo GUI | [![Downloads](https://img.shields.io/github/downloads/pzim-claude/nemo-actions/latest/mediainfo-gui@pzim-devdata.zip)](https://github.com/pzim-claude/nemo-actions/releases/latest) | [README](mediainfo-gui@pzim-devdata/README.md) |
| [📋 Paste into Document](#-paste-into-document) | Paste clipboard into a new document | [![Downloads](https://img.shields.io/github/downloads/pzim-claude/nemo-actions/latest/paste-into-document@pzim-devdata.zip)](https://github.com/pzim-claude/nemo-actions/releases/latest) | [README](paste-into-document@pzim-devdata/README.md) |
| [🖨️ Print File](#️-print-file) | Native GTK print dialog from Nemo | [![Downloads](https://img.shields.io/github/downloads/pzim-claude/nemo-actions/latest/print-native@pzim-devdata.zip)](https://github.com/pzim-claude/nemo-actions/releases/latest) | [README](print-native@pzim-devdata/README.md) |
| [🔄 Reload all Cinnamon Extensions](#-reload-all-cinnamon-extensions) | Reload extensions without restarting | [![Downloads](https://img.shields.io/github/downloads/pzim-claude/nemo-actions/latest/reload-all-extensions@pzim-devdata.zip)](https://github.com/pzim-claude/nemo-actions/releases/latest) | [README](reload-all-extensions@pzim-devdata/README.md) |
| [🧹 Remove Image Metadata](#-remove-image-metadata) | Strip EXIF, IPTC, XMP from images | [![Downloads](https://img.shields.io/github/downloads/pzim-claude/nemo-actions/latest/remove-image-metadata@pzim-devdata.zip)](https://github.com/pzim-claude/nemo-actions/releases/latest) | [README](remove-image-metadata@pzim-devdata/README.md) |

---

## 🖨️ Convert to PDF

Convert documents and images to PDF using LibreOffice, directly from the context menu.

**Requires:** `libreoffice` — `sudo apt install libreoffice`

```bash
curl -L "https://github.com/pzim-claude/nemo-actions/releases/latest/download/convert-to-pdf@pzim-devdata.zip" -o /tmp/convert-to-pdf.zip && unzip -o /tmp/convert-to-pdf.zip -d ~/.local/share/nemo/actions && rm /tmp/convert-to-pdf.zip && nemo -q
```

→ [Full documentation](convert-to-pdf@pzim-devdata/README.md)

---

## 😀 Copy an Emoticon

Quick access to commonly used emoticons with a zenity dialog, copy to clipboard in one click.

**Requires:** `zenity xclip gnome-characters` — `sudo apt install zenity xclip gnome-characters`

```bash
curl -L "https://github.com/pzim-claude/nemo-actions/releases/latest/download/copy-emoticon@pzim-devdata.zip" -o /tmp/copy-emoticon.zip && unzip -o /tmp/copy-emoticon.zip -d ~/.local/share/nemo/actions && rm /tmp/copy-emoticon.zip && nemo -q
```

→ [Full documentation](copy-emoticon@pzim-devdata/README.md)

---

## 🔒 Hidden Actions

Execute custom scripts placed in `~/.local/share/hidden_scripts/` via Ctrl+Right-click — keeps your context menu clean.

**Requires:** `python3-xlib zenity` — `sudo apt install python3-xlib zenity`

```bash
curl -L "https://github.com/pzim-claude/nemo-actions/releases/latest/download/hidden-actions@pzim-devdata.zip" -o /tmp/hidden-actions.zip && unzip -o /tmp/hidden-actions.zip -d ~/.local/share/nemo/actions && rm /tmp/hidden-actions.zip && nemo -q
```

→ [Full documentation](hidden-actions@pzim-devdata/README.md)

---

## 📥 Install Debian Package

Install `.deb` packages from the context menu using `apt`, with automatic dependency resolution.

**Requires:** `apt` (pre-installed on Debian-based systems)

```bash
curl -L "https://github.com/pzim-claude/nemo-actions/releases/latest/download/install-deb-package@pzim-devdata.zip" -o /tmp/install-deb.zip && unzip -o /tmp/install-deb.zip -d ~/.local/share/nemo/actions && rm /tmp/install-deb.zip && nemo -q
```

→ [Full documentation](install-deb-package@pzim-devdata/README.md)

---

## 🎬 Display Media Information

Display comprehensive technical metadata (codec, resolution, bitrate, EXIF, GPS…) using MediaInfo GUI.

**Requires:** `mediainfo-gui` — `sudo apt install mediainfo-gui`

```bash
curl -L "https://github.com/pzim-claude/nemo-actions/releases/latest/download/mediainfo-gui@pzim-devdata.zip" -o /tmp/mediainfo-gui.zip && unzip -o /tmp/mediainfo-gui.zip -d ~/.local/share/nemo/actions && rm /tmp/mediainfo-gui.zip && nemo -q
```

→ [Full documentation](mediainfo-gui@pzim-devdata/README.md)

---

## 📋 Paste into Document

Paste clipboard content (text, rich text, images) into a new document from the context menu. Supports odt, pdf, txt, md, html, json, yaml, csv, py, sh.

**Requires:** `python3 libreoffice` — `sudo apt install libreoffice`

```bash
curl -L "https://github.com/pzim-claude/nemo-actions/releases/latest/download/paste-into-document@pzim-devdata.zip" -o /tmp/paste-into-document.zip && unzip -o /tmp/paste-into-document.zip -d ~/.local/share/nemo/actions && rm /tmp/paste-into-document.zip && nemo -q
```

→ [Full documentation](paste-into-document@pzim-devdata/README.md)

---

## 🖨️ Print File

Open the native GTK print dialog for any file — identical to File > Print in gedit or evince, with full CUPS options.

**Requires:** `python3-gi` (pre-installed on most systems) — `sudo apt install python3-gi`

```bash
curl -L "https://github.com/pzim-claude/nemo-actions/releases/latest/download/print-native@pzim-devdata.zip" -o /tmp/print-native.zip && unzip -o /tmp/print-native.zip -d ~/.local/share/nemo/actions && rm /tmp/print-native.zip && nemo -q
```

→ [Full documentation](print-native@pzim-devdata/README.md)

---

## 🔄 Reload all Cinnamon Extensions

Reload all active Cinnamon extensions without restarting the desktop. No dependencies required.

```bash
curl -L "https://github.com/pzim-claude/nemo-actions/releases/latest/download/reload-all-extensions@pzim-devdata.zip" -o /tmp/reload-all-extensions.zip && unzip -o /tmp/reload-all-extensions.zip -d ~/.local/share/nemo/actions && rm /tmp/reload-all-extensions.zip && nemo -q
```

→ [Full documentation](reload-all-extensions@pzim-devdata/README.md)

---

## 🧹 Remove Image Metadata

Remove all EXIF, IPTC, XMP, GPS and other metadata from images. Supports 50+ formats including RAW.

**Requires:** `exiftool` — `sudo apt install exiftool`

```bash
curl -L "https://github.com/pzim-claude/nemo-actions/releases/latest/download/remove-image-metadata@pzim-devdata.zip" -o /tmp/remove-image-metadata.zip && unzip -o /tmp/remove-image-metadata.zip -d ~/.local/share/nemo/actions && rm /tmp/remove-image-metadata.zip && nemo -q
```

→ [Full documentation](remove-image-metadata@pzim-devdata/README.md)

---

## 📄 License

MIT — see [LICENSE](LICENSE)

## 👤 Author

[pzim-claude](https://github.com/pzim-claude)
