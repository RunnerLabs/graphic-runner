# Graphic Runner

Graphic Runner is a free offline desktop graphics studio for creating high-impact text, image, logo-vector, symbol, and print effects. The public beta is proprietary freeware, not open-source software.

## Download

Download this build from the [official v0.0.18 GitHub release](https://github.com/RunnerLabs/graphic-runner/releases/tag/v0.0.18).

- `GraphicRunnerInstallBeta.exe` — recommended Windows 10/11 installer.
- `GraphicRunnerInstallBeta.msi` — alternate Windows MSI installer.
- `graphicrunner_0.0.18-1_amd64.deb` — native Ubuntu/Debian x64 package.
- `GraphicRunner-Linux-x64-0.0.18.tar.gz` — portable native Linux x64 bundle.
- `SHA256SUMS.txt` — checksums for verifying every download.

Every package includes Graphic Runner's Java runtime. Users do not need to install Java separately.

## Windows installation

1. Download `GraphicRunnerInstallBeta.exe`.
2. Verify its SHA-256 checksum against `SHA256SUMS.txt`.
3. Run the installer and accept the beta license.
4. Because the beta is not digitally signed yet, Windows may show **Windows protected your PC**. After verifying the checksum, select **More info**, confirm the app name, and select **Run anyway**.

Do not disable Microsoft Defender or SmartScreen. Trusted code signing is the permanent fix for the unsigned-publisher warning.

## Native Linux installation

Graphic Runner v0.0.18 includes native x64 Linux builds produced on an Ubuntu 22.04 baseline. Wine and Bottles are no longer required.

### Ubuntu/Debian package

Download `graphicrunner_0.0.18-1_amd64.deb`, verify its checksum, then run:

```bash
sudo apt install ./graphicrunner_0.0.18-1_amd64.deb
```

Launch **GraphicRunner** from the desktop application menu.

### Portable Linux bundle

Download `GraphicRunner-Linux-x64-0.0.18.tar.gz`, verify it, then run:

```bash
tar -xzf GraphicRunner-Linux-x64-0.0.18.tar.gz
./GraphicRunner/bin/GraphicRunner
```

The portable bundle includes its own Java runtime but still needs a graphical Linux desktop, standard X11/font libraries, `libvulkan1`, and a current Vulkan-capable graphics driver for AI upscale. The DEB declares the Vulkan runtime automatically. Classic resize and the rest of the editor remain available if AI inference cannot start.

## Verify your download

For Graphic Runner v0.0.18 Java Beta:

```text
F4053FD6B3DF68B664212A2CAC90DFF416510976FF39BF30835918F2567B4C09  GraphicRunnerInstallBeta.exe
08D3E32842E066A868CC147E5B89B4CE03CC85259DDD2A16AA63FB9619DC65A5  GraphicRunnerInstallBeta.msi
1F1DF51BE88B4B8291826E1B7F5EAEC9F7A2BED50048A308B79DA8D5CF741563  graphicrunner_0.0.18-1_amd64.deb
CD5477F5E0BA3C9ADD3865B7C15E94E4EA0183D15226B3244A68FF01501E59BA  GraphicRunner-Linux-x64-0.0.18.tar.gz
```

On Windows:

```powershell
Get-FileHash .\GraphicRunnerInstallBeta.exe -Algorithm SHA256
```

On Linux:

```bash
sha256sum graphicrunner_0.0.18-1_amd64.deb
```

## Privacy and source protection

Graphic Runner operates locally and does not upload your artwork. This public repository contains only the website, user-facing documentation, and compiled release downloads. Application source code and private build files are not included.

## Acceptable use

Each installer includes `README_FIRST.txt`, `LICENSE.txt`, the EULA v2.1 presented for acceptance, and `THIRD-PARTY-NOTICES.txt`. Users are responsible for their content and must have the rights required for every image, font, logo, trademark, and other item they use. Users may share the official release link but may not redistribute, sell, rebrand, relabel, host, or pass off Graphic Runner as their own application.

## Support

Send product feedback through the [Graphic Runner Beta Feedback form](https://forms.gle/xRCnM3ARTG7ps8CYA).

Security reports and private feedback: `taskmaster@trunner.net`

© 2026 Patrick Jamison. All rights reserved.
