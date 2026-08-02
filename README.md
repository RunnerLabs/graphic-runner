# Graphic Runner

Graphic Runner is a free offline desktop graphics studio for creating high-impact text, image, logo-vector, symbol, and print effects. The public beta is proprietary freeware, not open-source software.

## Download

Download the current Windows and native Linux builds from the [official v0.0.19 GitHub release](https://github.com/RunnerLabs/graphic-runner/releases/tag/v0.0.19).

- `GraphicRunnerInstallBeta.exe` — recommended Windows 10/11 v0.0.19 installer.
- `GraphicRunnerInstallBeta.msi` — alternate Windows v0.0.19 MSI installer.
- `graphicrunner_0.0.19_amd64.deb` — native Ubuntu/Debian x64 package.
- `GraphicRunner-Linux-x64-0.0.19.tar.gz` — portable native Linux x64 bundle.
- `SHA256SUMS.txt` — Windows checksums.
- `SHA256SUMS-LINUX.txt` — Linux checksums.

Every package includes Graphic Runner's Java runtime. Users do not need to install Java separately.

## What is new in v0.0.19

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

1. Download `GraphicRunnerInstallBeta.exe`.
2. Verify its SHA-256 checksum against `SHA256SUMS.txt`.
3. Run the installer and accept the beta license.
4. Because the beta is not digitally signed yet, Windows may show **Windows protected your PC**. After verifying the checksum, select **More info**, confirm the app name, and select **Run anyway**.

Do not disable Microsoft Defender or SmartScreen. Trusted code signing is the permanent fix for the unsigned-publisher warning.

## Native Linux installation

Graphic Runner v0.0.19 includes native x64 Linux builds. Wine and Bottles are not required.

### Ubuntu/Debian package

Download `graphicrunner_0.0.19_amd64.deb`, verify its checksum, then run:

```bash
sudo apt install ./graphicrunner_0.0.19_amd64.deb
```

Launch **GraphicRunner** from the desktop application menu.

### Portable Linux bundle

Download `GraphicRunner-Linux-x64-0.0.19.tar.gz`, verify it, then run:

```bash
tar -xzf GraphicRunner-Linux-x64-0.0.19.tar.gz
./GraphicRunner/bin/GraphicRunner
```

The portable bundle includes its own Java runtime but still needs a graphical Linux desktop, standard X11/font libraries, `libvulkan1`, and a current Vulkan-capable graphics driver for AI upscale. The DEB declares the Vulkan runtime automatically. Classic resize and the rest of the editor remain available if AI inference cannot start.

## Verify your download

For Graphic Runner Windows v0.0.19 Java Beta:

```text
2E962CD69B94C71E910D6D4736E3E53BD3E8A7DDD942C82CAE2CDC45A82797B0  GraphicRunnerInstallBeta.exe
D6E48DDAABF9C3787FE2525E443DBA8D8E76A63DA46545D7434C09C29360AA4C  GraphicRunnerInstallBeta.msi
```

For the native Linux v0.0.19 build:

```text
86F2F540DAE922B000DF635F9F9E6B70D7F04D3C45D205548E51683A8FB7EC80  graphicrunner_0.0.19_amd64.deb
4946E8795377CA9FA31CAD051CDB82BFDC82D03705E92B3C7DA55256B468FF8B  GraphicRunner-Linux-x64-0.0.19.tar.gz
```

On Windows:

```powershell
Get-FileHash .\GraphicRunnerInstallBeta.exe -Algorithm SHA256
```

On Linux:

```bash
sha256sum graphicrunner_0.0.19_amd64.deb
```

## Privacy and source protection

Graphic Runner operates locally and does not upload your artwork. This public repository contains only the website, user-facing documentation, and compiled release downloads. Application source code and private build files are not included.

## Acceptable use

Each installer includes `README_FIRST.txt`, `LICENSE.txt`, the EULA v2.1 presented for acceptance, and `THIRD-PARTY-NOTICES.txt`. Users are responsible for their content and must have the rights required for every image, font, logo, trademark, and other item they use. Users may share the official release link but may not redistribute, sell, rebrand, relabel, host, or pass off Graphic Runner as their own application.

## Support

Send product feedback through the [Graphic Runner Beta Feedback form](https://forms.gle/xRCnM3ARTG7ps8CYA).

Security reports and private feedback: `taskmaster@trunner.net`

© 2026 Patrick Jamison. All rights reserved.
