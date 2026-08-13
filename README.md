# Graphic Runner

Graphic Runner is a free offline desktop graphics studio for text, images,
logo-vector artwork, symbols, sketching, and print effects. The public beta is
proprietary freeware, not open-source software.

## Download v0.0.20.2

Download the current Windows and native Linux builds from the
[official v0.0.20.2 release](https://github.com/RunnerLabs/graphic-runner/releases/tag/v0.0.20.2).

- `GraphicRunner-0.0.20.2-Windows-Setup.exe` - recommended Windows 10/11 installer.
- `graphicrunner_0.0.20.2_amd64.deb` - native Ubuntu/Debian x64 installer.
- `GraphicRunner-Linux-x64-0.0.20.2.tar.gz` - portable native Linux x64 bundle.
- `SHA256SUMS_v0.0.20.2.txt` - checksums for every v0.0.20.2 download.

Every package includes Graphic Runner's Java runtime. Users do not need to
install Java separately.

## What is new in v0.0.20.2

![Graphic Runner v0.0.20.2 feature updates](assets/GraphicRunner-v0.0.20.2-Updates.png)

- AI-enhanced object selection, selection cleanup, feathering, and local
  inpainting.
- Dedicated Paint Color eyedropper in Image mode: press **Pick**, then sample
  an exact visible canvas color to make it the active brush color.
- Speed Form Mode with tapered industrial-sketch profiles, round or block
  marker tips, and exclusive tool switching so only one canvas tool is active.
- Independent, movable, resizable artboards with separate layer stacks and
  single or batch export.
- Persistent selections, polygon selection, invert selection, masking actions,
  layer locking, clipping, and faster layer interaction.
- Direct image corner resizing, cropping, alignment, rotation, flipping, and
  Convert to Curves handoff.
- Paint, eraser, smudge, clone, trace rulers, gradients, independent strokes,
  expanded dithering/glow, and additional themes.
- Print True 4000 px preview, Runner Developer finishing, performance diagnostics,
  native Linux packaging, and source-free public downloads.
- Selected painting now responds immediately and remains attached to the intended
  layer after the stroke, including above a separate solid-plane layer.

## Windows installation

1. Download `GraphicRunner-0.0.20.2-Windows-Setup.exe`.
2. Verify its SHA-256 checksum against `SHA256SUMS_v0.0.20.2.txt`.
3. Run the Setup EXE. It installs Graphic Runner for the current user, adds a
   Start-menu shortcut, and registers a normal Windows uninstaller.
4. Accept the beta license when Graphic Runner opens.
5. Because this beta is not digitally signed yet, Windows may show **Windows
   protected your PC**. After verifying the checksum, select **More info**,
   confirm the app name, and select **Run anyway**.

Do not disable Microsoft Defender or SmartScreen. Trusted code signing is the
permanent fix for the unsigned-publisher warning.

## Native Linux installation

Graphic Runner v0.0.20.2 includes native x64 Linux builds. Wine and Bottles are
not required.

### Ubuntu/Debian package

Download `graphicrunner_0.0.20.2_amd64.deb`, verify its checksum, then run:

```bash
sudo apt install ./graphicrunner_0.0.20.2_amd64.deb
```

Launch **GraphicRunner** from the desktop application menu.

### Portable Linux bundle

Download `GraphicRunner-Linux-x64-0.0.20.2.tar.gz`, verify it, then run:

```bash
tar -xzf GraphicRunner-Linux-x64-0.0.20.2.tar.gz
./GraphicRunner/bin/GraphicRunner
```

The portable bundle includes Java but still needs a graphical Linux desktop
and the normal X11/font libraries. The DEB declares its runtime dependencies.

## Verify your download

```text
6F514F7F0DA7F709400226E88596D013985C62BB141F2DAE436CB9FE12A34DB3  GraphicRunner-0.0.20.2-Windows-Setup.exe
EB244EAD75CC49686B7A02341EC4388FA17A50A8DF97009AF8AEA4F1949F1CE2  graphicrunner_0.0.20.2_amd64.deb
08701B73B46E5C56DBD535897B8D01711226168328D4378B7128139F6250FBAA  GraphicRunner-Linux-x64-0.0.20.2.tar.gz
```

Windows:

```powershell
Get-FileHash .\GraphicRunner-0.0.20.2-Windows-Setup.exe -Algorithm SHA256
```

Linux:

```bash
sha256sum graphicrunner_0.0.20.2_amd64.deb
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
