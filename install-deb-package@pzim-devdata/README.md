# Install Debian Package

Install `.deb` packages directly from Nemo's context menu with automatic dependency resolution via `apt`.

![screenshot](screenshot-auto_1769727347.png)

## Requirements

- `apt` (pre-installed on Debian-based systems)

## Installation

### One-line install

```bash
curl -L "https://github.com/pzim-claude/nemo-actions/releases/latest/download/install-deb-package@pzim-devdata.zip" -o /tmp/install-deb.zip && \
unzip -o /tmp/install-deb.zip -d /tmp/install-deb-install && \
cp -rf /tmp/install-deb-install/install-deb-package@pzim-devdata/. ~/.local/share/nemo/actions/install-deb-package@pzim-devdata/ && \
rm -rf /tmp/install-deb.zip /tmp/install-deb-install && \
nemo -q
```

### Manual install

Download [install-deb-package@pzim-devdata.zip](https://github.com/pzim-claude/nemo-actions/releases/latest/download/install-deb-package@pzim-devdata.zip), extract and copy contents:

```bash
unzip install-deb-package@pzim-devdata.zip -d /tmp/install-deb-install && \
cp -rf /tmp/install-deb-install/install-deb-package@pzim-devdata/. ~/.local/share/nemo/actions/install-deb-package@pzim-devdata/ && \
rm -rf /tmp/install-deb-install && \
nemo -q
```

## Usage

Right-click on any `.deb` file → select **"Install Debian Package"**. A terminal opens, enter your password when prompted — dependencies are resolved and installed automatically.

## Why `apt` instead of `dpkg -i`?

`apt install` automatically downloads and installs missing dependencies, whereas `dpkg -i` fails if dependencies are not already present.

## Author

[pzim-claude](https://github.com/pzim-claude)
