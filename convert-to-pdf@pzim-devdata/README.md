# Convert to PDF

Convert documents and images to PDF directly from the Nemo file manager context menu, using LibreOffice.

## Requirements

- LibreOffice

```bash
sudo apt install libreoffice
```

## Installation

### One-line install

```bash
curl -L "https://github.com/pzim-claude/nemo-actions/releases/latest/download/convert-to-pdf@pzim-devdata.zip" -o /tmp/convert-to-pdf.zip && unzip -o /tmp/convert-to-pdf.zip -d ~/.local/share/nemo/actions && rm /tmp/convert-to-pdf.zip && nemo -q
```

### Manual install

Download [convert-to-pdf@pzim-devdata.zip](https://github.com/pzim-claude/nemo-actions/releases/latest/download/convert-to-pdf@pzim-devdata.zip), then:

```bash
unzip convert-to-pdf@pzim-devdata.zip -d ~/.local/share/nemo/actions
nemo -q
```

## Usage

Right-click on any supported file and select **"Convert to PDF"**.

## Supported formats

**Documents:** odt, ods, odp, odg, odf, doc, docx, xls, xlsx, ppt, pptx, rtf, txt, html, htm, csv

**Images:** jpg, jpeg, png, gif, bmp, tif, tiff, svg, webp, pcx, tga, pbm, pgm, ppm, eps, wmf, emf

## Author

[pzim-claude](https://github.com/pzim-claude)
