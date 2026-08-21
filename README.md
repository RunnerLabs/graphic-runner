# Graphic Runner

Graphic Runner is a free offline desktop graphics studio for text, images,
logo-vector artwork, symbols, sketching, and print effects. The public beta is
proprietary freeware, not open-source software.

## Download v0.0.21

Download the current Windows and native Linux builds from the
[official v0.0.21 release](https://github.com/RunnerLabs/graphic-runner/releases/tag/v0.0.21).

- `GraphicRunner-0.0.21-Windows-Setup.exe` - recommended Windows 10/11 installer.
- `graphicrunner_0.0.21-1_debian13_amd64.deb` - native Debian 13 x86-64 installer.
- `GraphicRunner-Linux-x64-0.0.21.tar.gz` - portable native Linux x64 bundle.
- `SHA256SUMS_v0.0.21.txt` - checksums for every v0.0.21 download.

Every package includes Graphic Runner's Java runtime. Users do not need to
install Java separately.

## What is new in v0.0.21

- **Runner Text Track** flows editable text inside a selection or around its
  outline, with Style Type and Type Lab node-editing handoff.
- **Advanced selections** add a Bezier Pen tool, replace/add/subtract modes,
  locked selections, AI-enhanced object selection, and undoable raster strokes.
- **Faster canvas work** adds bounded High/Ultra render caching, responsive
  masking and erasing, faster project saves, and local performance diagnostics.
- **Speed Form and drawing guides** add editable start/middle/end stroke handles,
  smoother high-quality output, flex rulers, symmetry, perspective grids, and
  perspective shading.
- **Layers and artboards** add clearer multi-layer selection, selected/all merge,
  clipping, independent movable artboards, batch export, labels, and color tags.
- **Deeper styling** adds a standalone Pixel Engine, Gaussian/Focus/Speed blur,
  text/vector gradients and strokes, selection strokes, and composition overlays.
- **Safer editable projects** add Save As, quicker `.grdoc` saves, restricted
  document loading, UI recovery tools, and source-free native packages.
- AI-enhanced object selection, inpainting, and upscaling remain fully local.

## Windows installation

1. Download `GraphicRunner-0.0.21-Windows-Setup.exe`.
2. Verify its SHA-256 checksum against `SHA256SUMS_v0.0.21.txt`.
3. Run the Setup EXE. It installs Graphic Runner for the current user, adds a
   Start-menu shortcut, and registers a normal Windows uninstaller.
4. Accept the beta license when Graphic Runner opens.
5. Because this beta is not digitally signed yet, Windows may show **Windows
   protected your PC**. After verifying the checksum, select **More info**,
   confirm the app name, and select **Run anyway**.

Do not disable Microsoft Defender or SmartScreen. Trusted code signing is the
permanent fix for the unsigned-publisher warning.

## Native Linux installation

Graphic Runner v0.0.21 includes native x64 Linux builds. Wine and Bottles are
not required.

### Debian 13 package

Download `graphicrunner_0.0.21-1_debian13_amd64.deb`, verify its checksum, then run:

```bash
cd ~/Downloads
sudo apt install ./graphicrunner_0.0.21-1_debian13_amd64.deb
```

Launch **GraphicRunner** from the desktop application menu.

This DEB is built for Debian 13 on x86-64. Other Debian-based
distributions may work but are not yet validated. Ubuntu uses different runtime
package names and should not use this Debian 13 build. Fedora, openSUSE, Arch,
SteamOS, ARM devices, and other non-Debian systems are not supported by this
DEB. Use the portable x64 bundle where its required desktop libraries are
available. AI upscaling also requires a Vulkan-capable GPU and current driver.

### Portable Linux bundle

Download `GraphicRunner-Linux-x64-0.0.21.tar.gz`, verify it, then run:

```bash
tar -xzf GraphicRunner-Linux-x64-0.0.21.tar.gz
./GraphicRunner/bin/GraphicRunner
```

The portable bundle includes Java but still needs a graphical Linux desktop
and the normal X11/font libraries. The DEB declares its runtime dependencies.

## Verify your download

```text
2A4A67C421FA42C4B744A8FC472FE4ED4C0E4D89142FCCB8973AFF6D05D3B2A5  GraphicRunner-0.0.21-Windows-Setup.exe
D2FC93BF1B78F25872C82BD61E8486AE4A7EB33A1378BF7C6FA7BB1AA92EF25B  graphicrunner_0.0.21-1_debian13_amd64.deb
9948592D0D39B505C5049FD746B41EDC35AA12C20781C3AD5C013717DAE5D189  GraphicRunner-Linux-x64-0.0.21.tar.gz
```

Windows:

```powershell
Get-FileHash .\GraphicRunner-0.0.21-Windows-Setup.exe -Algorithm SHA256
```

Linux:

```bash
sha256sum graphicrunner_0.0.21-1_debian13_amd64.deb
```

## Privacy and source protection

Graphic Runner operates locally and does not upload artwork. This public
repository contains only the website, user-facing documentation, and compiled
release downloads. Application source code and private build files are not
included.

## AI-enhanced features, privacy, and acceptance

By installing, launching, or using Graphic Runner, including any AI-enhanced
feature, you acknowledge and agree to the terms included with the application.
AI-enhanced features perform only their described editing functions: helping
select objects, reconstructing a selected image area, and enhancing image
resolution when the user explicitly requests those actions.

Graphic Runner does not use AI-enhanced features to collect personal data,
upload artwork, monitor activity, build profiles, train on user content, or
retain user content for another purpose. Processing stays on the user's device.
No account, telemetry system, cloud service, or remote AI service is involved.
Only the local acceptance record and app settings are stored automatically;
files are otherwise saved when the user chooses to save or export them. Users
remain responsible for reviewing results and for the content they create,
import, publish, or distribute. The included license contains the complete
terms governing use of Graphic Runner.

## Acceptable use

Each package includes `README_FIRST.txt`, `LICENSE.txt`, the EULA v2.1,
`SECURITY.md`, and `THIRD-PARTY-NOTICES.txt`. Users are responsible for their
content and must have the rights required for every image, font, logo,
trademark, and other item they use. Users may share the official release link
but may not redistribute, sell, rebrand, relabel, host, or pass off Graphic
Runner as their own application.

## Support

Send product feedback through the
[Graphic Runner Beta Feedback form](https://forms.gle/xRCnM3ARTG7ps8CYA).

Security reports and private feedback: `taskmaster@trunner.net`

Copyright 2026 Patrick Jamison. All rights reserved.
