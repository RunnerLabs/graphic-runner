# Graphic Runner

Graphic Runner is a free offline desktop graphics studio for text, images,
logo-vector artwork, symbols, sketching, merchandise, and print effects. The
public beta is proprietary freeware, not open-source software.

## Download v0.0.23 Beta

Download the Photo Runner, Contour Flow & Masking update from the
[official v0.0.23 release](https://github.com/RunnerLabs/graphic-runner/releases/tag/v0.0.23).

- `GraphicRunner-0.0.23-Windows-Setup.exe` — recommended Windows 10/11 installer.
- `graphicrunner_0.0.23-1_amd64.deb` — native Ubuntu 22.04+ x64 installer with declared desktop dependencies.
- `GraphicRunner-Linux-x64-0.0.23.tar.gz` — portable native Linux x64 bundle.
- `SHA256SUMS_v0.0.23.txt` — checksums for every download.

Every package includes Graphic Runner's Java runtime and offline AI models.
Users do not need to install Java separately.

## New in v0.0.23

- Photo Runner adjustments, fine grain, luminance-preserving color balance, and selective HSL.
- Contour Flow and Signal Track variants that stack with dithering and Photo Runner.
- Source colors by default, adjustable palette mixing, transparent gaps, and finer line spacing.
- Searchable Main Glow and finished-layer blur with Preserve Alpha.
- Larger masking and Pattern Maker controls, crop locking, Fit Canvas to Image, and accessible DTF preparation.
- Cached mask effects and coalesced preview requests for more responsive masking.
- Explicit Linux desktop, Vulkan-loader, and OpenMP dependencies.

[Full v0.0.23 release notes](RELEASE_NOTES_v0.0.23-beta.md)

## Creative Control features

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
- **Earlier creative controls:** native vector text-to-curves, non-destructive
  four-corner perspective for image/text/vector layers, draggable and detachable
  right tabs, Vector planes and templates, faster Speed Form node editing,
  improved Mock Runner cylinder controls, Effects search, Dark Gray and Task
  themes, a UI-only blue-light filter, and repaired offline AI Object Selection.

## Windows installation

1. Download `GraphicRunner-0.0.23-Windows-Setup.exe`.
2. Verify its SHA-256 checksum against `SHA256SUMS_v0.0.23.txt`.
3. Run Setup, then accept the beta license when Graphic Runner opens.
4. This beta is not digitally signed yet, so Windows may show **Windows
   protected your PC**. After verifying the checksum, select **More info**,
   confirm the app name, and select **Run anyway**.

Do not disable Microsoft Defender or SmartScreen. Trusted code signing is the
permanent fix for the unsigned-publisher warning.

## Native Linux installation

Wine and Bottles are not required. For Ubuntu 22.04 or newer:

```bash
sudo apt install ./graphicrunner_0.0.23-1_amd64.deb
```

For the portable bundle:

```bash
tar -xzf GraphicRunner-Linux-x64-0.0.23.tar.gz
./GraphicRunner/bin/GraphicRunner
```

The DEB includes a verified Temurin Java runtime and declares its desktop dependencies, including fonts, X11, audio, and GTK with modern t64 package alternatives. The portable bundle needs the same system libraries. Both formats were tested on Ubuntu 22.04 and 26.04.

Native AI upscaling additionally needs `libvulkan1`, `libgomp1`, and a compatible Vulkan device/driver. These are optional for the core editor; GPU upscaling is not guaranteed on every system.

## Verify your download

```text
68A175CC963050E6921B9A655F7764D0A20B0F43DB71A5F6955D7D8D60880A8F  GraphicRunner-0.0.23-Windows-Setup.exe
465BDCE1F1F83679F0965657B1324560033027FD85D39582F32B47C3FD7D4DC2  graphicrunner_0.0.23-1_amd64.deb
C5D820966DF50F046213964EE08B7A278BB19A85444469CC4EFD3E4DA05245A7  GraphicRunner-Linux-x64-0.0.23.tar.gz
```

Windows: `Get-FileHash .\GraphicRunner-0.0.23-Windows-Setup.exe -Algorithm SHA256`

Linux: `sha256sum graphicrunner_0.0.23-1_amd64.deb`

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
