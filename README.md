# Graphic Runner

Graphic Runner is a free offline desktop graphics studio for text, images,
logo-vector artwork, symbols, sketching, merchandise, and print effects. The
public beta is proprietary freeware, not open-source software.

## Download v0.0.22 Beta

Download the Creative Control Update from the
[official v0.0.22 release](https://github.com/RunnerLabs/graphic-runner/releases/tag/v0.0.22).

- `GraphicRunner-0.0.22-Windows-Setup.exe` — recommended Windows 10/11 installer.
- `GraphicRunner-0.0.22-Windows-Installer.msi` — Windows managed-install package.
- `graphicrunner_0.0.22_amd64.deb` — native Ubuntu/Debian x64 installer.
- `GraphicRunner-Linux-x64-0.0.22.tar.gz` — portable native Linux x64 bundle.
- `SHA256SUMS_v0.0.22.txt` — checksums for every download.

Every package includes Graphic Runner's Java runtime and offline AI models.
Users do not need to install Java separately.

## Creative Control Update

- **Arrange the workspace your way:** move tool panels by dragging their `//`
  headings, or use Settings > UI Manager to reorder, move, hide, restore, and
  reset tools across tabs from one compact view.
- **Stronger layer control:** visible black-and-white mask thumbnails, layer
  grouping and ungrouping, collapsible nesting, unnesting, drag-out nesting,
  clearer layer rows, and safer new-layer behavior for solid planes and paint.
- **Faster pixel work:** deeper zoom for pixel editing, Paint Bucket (`G`) fills,
  Polygon Selection (`S`), selection-paint Undo, corrected blank-canvas cleanup,
  tighter transform bounds, smoother movement, and safer rotation.
- **Sketch and Image Trace:** centerline strokes, straight/sharp Geometry Trace,
  filled silhouettes, clean black-and-white PNG Image Trace, editable curves,
  marquee node selection, mass delete, and group movement of selected nodes.
- **Local AI Auto Polish:** verified MIT-licensed TEED inference runs entirely
  offline, reconnects and smooths sketch edges, and now preserves fine line
  weight instead of making every trace heavy.
- **Export Runner control:** choose which layers animate in the checked-layer
  preview, keep other layers static, export a single animated layer when needed,
  cap GIF length at five seconds, and begin with GIF previews safely off.
- **DTF and color workflow:** white is the creation default, regular color
  pickers share the Canvas Brushes primary color, DTF remains independent, and
  its threshold is directly adjustable.
- **More quality-of-life improvements:** current social, screen, mobile, and
  print canvas templates; scroll position retention during panel moves; Noise in
  Effects; unlocked text-box dimensions; improved sizing and clipped-label
  layouts; and Image mode as the default workspace and first layer.

## Windows installation

1. Download `GraphicRunner-0.0.22-Windows-Setup.exe`.
2. Verify its SHA-256 checksum against `SHA256SUMS_v0.0.22.txt`.
3. Run Setup, then accept the beta license when Graphic Runner opens.
4. This beta is not digitally signed yet, so Windows may show **Windows
   protected your PC**. After verifying the checksum, select **More info**,
   confirm the app name, and select **Run anyway**.

Do not disable Microsoft Defender or SmartScreen. Trusted code signing is the
permanent fix for the unsigned-publisher warning.

## Native Linux installation

Wine and Bottles are not required. For Ubuntu/Debian:

```bash
sudo apt install ./graphicrunner_0.0.22_amd64.deb
```

For the portable bundle:

```bash
tar -xzf GraphicRunner-Linux-x64-0.0.22.tar.gz
./GraphicRunner/bin/GraphicRunner
```

The DEB declares its runtime dependencies. Portable users need a graphical x64
Linux desktop plus `libvulkan1` and `libgomp1` for the bundled AI upscaler.

## Verify your download

```text
632BBB53FC064BA2F73CE7E31AA28CA4808AD33046B4279BA7982C72F2C85FE0  GraphicRunner-0.0.22-Windows-Installer.msi
77B0F4E047DC2463BAFF73729B825EC33B6CE201214CC37DD8187D44268546FB  GraphicRunner-0.0.22-Windows-Setup.exe
AC98F981679113A026C5ADB9F0FF72264C9C6C7A861D3E73EDC6557BBC166422  graphicrunner_0.0.22_amd64.deb
584BE8E7B1B6CEF203802126361905DD187BF26B246775D48FB610BB4B4E6434  GraphicRunner-Linux-x64-0.0.22.tar.gz
```

Windows: `Get-FileHash .\GraphicRunner-0.0.22-Windows-Setup.exe -Algorithm SHA256`

Linux: `sha256sum graphicrunner_0.0.22_amd64.deb`

## Privacy and source protection

Graphic Runner operates locally and does not upload artwork. Local AI features
perform only the editing action the user requests; there is no account,
telemetry, remote inference, training on user content, or cloud storage.

This public repository contains only the website, user-facing documentation,
and compiled release downloads. Application source code and private build files
are not included.

Each package includes `README_FIRST.txt`, `LICENSE.txt`, the EULA,
`SECURITY.md`, AI supply-chain records, and `THIRD-PARTY-NOTICES.txt`. Users are
responsible for their content and must have the rights required for everything
they import, create, publish, or sell.

## Support

[Graphic Runner Beta Feedback](https://forms.gle/xRCnM3ARTG7ps8CYA)

Security reports and private feedback: `taskmaster@trunner.net`

Copyright 2026 Patrick Jamison. All rights reserved.
