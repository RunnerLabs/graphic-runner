# Graphic Runner

Graphic Runner is a free offline desktop graphics studio for creating high-impact text, image, logo-vector, symbol, and print effects. The public beta is proprietary freeware, not open-source software.

## Download

Download the current Windows and native Linux builds from the [official v0.0.19.1 GitHub release](https://github.com/RunnerLabs/graphic-runner/releases/tag/v0.0.19.1).

- `GraphicRunner-0.0.19.1-Windows-Portable.zip` — Windows 10/11 portable package.
- `graphicrunner_0.0.19.1_amd64.deb` — native Ubuntu/Debian x64 package.
- `GraphicRunner-Linux-x64-0.0.19.1.tar.gz` — portable native Linux x64 bundle.
- `SHA256SUMS.txt` — checksums for every v0.0.19.1 download.

Every package includes Graphic Runner's Java runtime. Users do not need to install Java separately.

## What is new in v0.0.19.1

- **Ultra / Print True** preview renders through the same 4000 px path as the
  4x print export, then downsamples it for a much closer on-canvas match.
- Bicubic image transforms, fractional placement, anti-aliased masks, text,
  vectors, strokes, and consistent high-quality color/alpha interpolation.
- A new regression test protects transformed diagonal edges from falling back
  to jagged nearest-neighbor rendering.
- This maintenance release keeps the public v0.0.19 feature set and does not
  contain the private v0.0.20 object-selector work.

The v0.0.19 feature set also includes:

- Standard, High, and Ultra canvas-preview quality.
- Camera Raw finishing with sharpen, clarity, brightness, tones, color grading,
  luminance denoise, and color denoise.
- Alignment, 90-degree rotation, horizontal/vertical flipping, optional
  artboards, and a dedicated Layout panel.
- Borderless alpha canvas, universal black-and-white filter, drag-and-drop image
  import, and clipboard paste.
- Smoother paint strokes with stable opacity, `B` brush shortcut, improved
  loading lock, and clearer bottom-inserted blank layers.

## Windows installation

1. Download `GraphicRunner-0.0.19.1-Windows-Portable.zip`.
2. Verify its SHA-256 checksum against `SHA256SUMS.txt`.
3. Extract the ZIP, open its `GraphicRunner` folder, and run `GraphicRunner.exe`.
4. Accept the beta license when Graphic Runner opens.
5. Because the beta is not digitally signed yet, Windows may show **Windows protected your PC**. After verifying the checksum, select **More info**, confirm the app name, and select **Run anyway**.

Do not disable Microsoft Defender or SmartScreen. Trusted code signing is the permanent fix for the unsigned-publisher warning.

## Native Linux installation

Graphic Runner v0.0.19.1 includes native x64 Linux builds. Wine and Bottles are not required.

### Ubuntu/Debian package

Download `graphicrunner_0.0.19.1_amd64.deb`, verify its checksum, then run:

```bash
sudo apt install ./graphicrunner_0.0.19.1_amd64.deb
```

Launch **GraphicRunner** from the desktop application menu.

### Portable Linux bundle

Download `GraphicRunner-Linux-x64-0.0.19.1.tar.gz`, verify it, then run:

```bash
tar -xzf GraphicRunner-Linux-x64-0.0.19.1.tar.gz
./GraphicRunner/bin/GraphicRunner
```

The portable bundle includes its own Java runtime but still needs a graphical Linux desktop, standard X11/font libraries, `libvulkan1`, and a current Vulkan-capable graphics driver for AI upscale. The DEB declares the Vulkan runtime automatically. Classic resize and the rest of the editor remain available if AI inference cannot start.

## Verify your download

For Graphic Runner v0.0.19.1:

```text
15709E64C4002FAA359F9ED88219EA1C13EDEF198F73CD6AF36A0444FB38F15D  GraphicRunner-0.0.19.1-Windows-Portable.zip
33C7289C9324C369E3A27F4C8675FE87D424084871E6A4FE1B76E576CF4E1FE8  graphicrunner_0.0.19.1_amd64.deb
96A1531D682BB704809A8DE5364FE04DA8A454B34612011365A39E6F85F49060  GraphicRunner-Linux-x64-0.0.19.1.tar.gz
```

On Windows:

```powershell
Get-FileHash .\GraphicRunner-0.0.19.1-Windows-Portable.zip -Algorithm SHA256
```

On Linux:

```bash
sha256sum graphicrunner_0.0.19.1_amd64.deb
```

## Privacy and source protection

Graphic Runner operates locally and does not upload your artwork. This public repository contains only the website, user-facing documentation, and compiled release downloads. Application source code and private build files are not included.

## Acceptable use

Each installer includes `README_FIRST.txt`, `LICENSE.txt`, the EULA v2.1 presented for acceptance, and `THIRD-PARTY-NOTICES.txt`. Users are responsible for their content and must have the rights required for every image, font, logo, trademark, and other item they use. Users may share the official release link but may not redistribute, sell, rebrand, relabel, host, or pass off Graphic Runner as their own application.

## Support

Send product feedback through the [Graphic Runner Beta Feedback form](https://forms.gle/xRCnM3ARTG7ps8CYA).

Security reports and private feedback: `taskmaster@trunner.net`

© 2026 Patrick Jamison. All rights reserved.
