# Graphic Runner

Graphic Runner is a free offline desktop graphics studio for text, images,
logo-vector artwork, symbols, sketching, merchandise, and print effects. The
public beta is proprietary freeware, not open-source software.

## Download v0.0.22.3 Beta

Download the Creative Control Update from the
[official v0.0.22.3 release](https://github.com/RunnerLabs/graphic-runner/releases/tag/v0.0.22.3).

- `GraphicRunner-0.0.22.3-Windows-Setup.exe` — recommended Windows 10/11 installer.
- `graphicrunner_0.0.22.3-2_amd64.deb` — dependency-controlled native Ubuntu/Debian x64 installer.
- `GraphicRunner-Linux-x64-0.0.22.3.tar.gz` — portable native Linux x64 bundle.
- `SHA256SUMS_v0.0.22.3.txt` — checksums for every download.

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
- **v0.0.22.3 refinements:** native vector text-to-curves, non-destructive
  four-corner perspective for image/text/vector layers, draggable and detachable
  right tabs, Vector planes and templates, faster Speed Form node editing,
  improved Mock Runner cylinder controls, Effects search, Dark Gray and Task
  themes, a UI-only blue-light filter, and repaired offline AI Object Selection.

## Windows installation

1. Download `GraphicRunner-0.0.22.3-Windows-Setup.exe`.
2. Verify its SHA-256 checksum against `SHA256SUMS_v0.0.22.3.txt`.
3. Run Setup, then accept the beta license when Graphic Runner opens.
4. This beta is not digitally signed yet, so Windows may show **Windows
   protected your PC**. After verifying the checksum, select **More info**,
   confirm the app name, and select **Run anyway**.

Do not disable Microsoft Defender or SmartScreen. Trusted code signing is the
permanent fix for the unsigned-publisher warning.

## Native Linux installation

Wine and Bottles are not required. For Ubuntu/Debian:

```bash
sudo apt install ./graphicrunner_0.0.22.3-2_amd64.deb
```

For the portable bundle:

```bash
tar -xzf GraphicRunner-Linux-x64-0.0.22.3.tar.gz
./GraphicRunner/bin/GraphicRunner
```

The DEB declares its runtime dependencies. Portable users need a graphical x64
Linux desktop plus `libvulkan1` and `libgomp1` for the bundled AI upscaler.

## Verify your download

```text
28D2F616BA4BBBF9D2F1EC6DC0594FDCBC927DB4FAC29976068B9916A05F25DD  GraphicRunner-0.0.22.3-Windows-Setup.exe
972B7931E35D25952DD51E2209E22F340CA26ED20BBF64CF3D66C91B1AA451E9  graphicrunner_0.0.22.3-2_amd64.deb
8D92E7E6635730631467846A0C31E79B66578DE80950F2E10B83271782499DC3  GraphicRunner-Linux-x64-0.0.22.3.tar.gz
```

Windows: `Get-FileHash .\GraphicRunner-0.0.22.3-Windows-Setup.exe -Algorithm SHA256`

Linux: `sha256sum graphicrunner_0.0.22.3-2_amd64.deb`

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
