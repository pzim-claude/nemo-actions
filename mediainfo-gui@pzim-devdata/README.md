# Display Media Information

Display comprehensive technical metadata about media files directly from Nemo's context menu, using MediaInfo GUI.

## Requirements

- `mediainfo-gui`

```bash
sudo apt install mediainfo-gui
```

## Installation

### One-line install

```bash
curl -L "https://github.com/pzim-claude/nemo-actions/releases/latest/download/mediainfo-gui@pzim-devdata.zip" -o /tmp/mediainfo-gui.zip && \
unzip -o /tmp/mediainfo-gui.zip -d /tmp/mediainfo-gui-install && \
mv /tmp/mediainfo-gui-install/mediainfo-gui@pzim-devdata/* ~/.local/share/nemo/actions/ && \
rm -rf /tmp/mediainfo-gui.zip /tmp/mediainfo-gui-install && \
nemo -q
```

### Manual install

Download [mediainfo-gui@pzim-devdata.zip](https://github.com/pzim-claude/nemo-actions/releases/latest/download/mediainfo-gui@pzim-devdata.zip), extract and move contents:

```bash
unzip mediainfo-gui@pzim-devdata.zip -d /tmp/mediainfo-gui-install && \
mv /tmp/mediainfo-gui-install/mediainfo-gui@pzim-devdata/* ~/.local/share/nemo/actions/ && \
rm -rf /tmp/mediainfo-gui-install && \
nemo -q
```

## Usage

Right-click on any media file → select **"Display Media Information"**. MediaInfo GUI opens with full technical details: codec, resolution, frame rate, bitrate, audio channels, sample rate, EXIF data, GPS, and more.

## Supported formats

**Video:** MPEG-4, MKV, AVI, MOV, WMV, WebM, MXF, FLV, and more

**Audio:** MP3, AAC, FLAC, OGG, AC3, DTS, WAV, WMA, and more

**Images:** JPEG, PNG, TIFF, WebP, HEIF, BMP, DNG, and more

**Subtitles:** SRT, SSA/ASS, VobSub, WebVTT, TTML

## Author

[pzim-claude](https://github.com/pzim-claude)
