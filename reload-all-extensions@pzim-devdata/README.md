# Reload all Cinnamon Extensions

Reload all active Cinnamon extensions without restarting the desktop environment, directly from Nemo's context menu.

## Requirements

No additional dependencies — uses built-in Cinnamon tools.

## Installation

### One-line install

```bash
curl -L "https://github.com/pzim-claude/nemo-actions/releases/latest/download/reload-all-extensions@pzim-devdata.zip" -o /tmp/reload-all-extensions.zip && \
unzip -o /tmp/reload-all-extensions.zip -d /tmp/reload-all-extensions-install && \
mv /tmp/reload-all-extensions-install/reload-all-extensions@pzim-devdata/* ~/.local/share/nemo/actions/ && \
rm -rf /tmp/reload-all-extensions.zip /tmp/reload-all-extensions-install && \
nemo -q
```

### Manual install

Download [reload-all-extensions@pzim-devdata.zip](https://github.com/pzim-claude/nemo-actions/releases/latest/download/reload-all-extensions@pzim-devdata.zip), extract and move contents:

```bash
unzip reload-all-extensions@pzim-devdata.zip -d /tmp/reload-all-extensions-install && \
mv /tmp/reload-all-extensions-install/reload-all-extensions@pzim-devdata/* ~/.local/share/nemo/actions/ && \
rm -rf /tmp/reload-all-extensions-install && \
nemo -q
```

## Usage

Right-click anywhere in Nemo → select **"Reload all Cinnamon extensions"**. All active extensions are temporarily disabled then re-enabled, forcing Cinnamon to reload their code.

## Author

[pzim-claude](https://github.com/pzim-claude)
