# Graphic Runner

Graphic Runner is a free offline desktop graphics studio for creating high-impact text, image, logo-vector, symbol, and print effects. The public beta is proprietary freeware, not open-source software.

## Download

Download the latest build from the [official GitHub release](https://github.com/RunnerLabs/graphic-runner/releases/latest).

- `GraphicRunnerInstallBeta.exe` — recommended Windows 10/11 installer.
- `GraphicRunnerInstallBeta.msi` — alternate Windows MSI installer.
- `graphicrunner_0.0.17-1_amd64.deb` — native Ubuntu/Debian x64 package.
- `GraphicRunner-Linux-x64-0.0.17.tar.gz` — portable native Linux x64 bundle.
- `SHA256SUMS.txt` — checksums for verifying every download.

Every package includes Graphic Runner's Java runtime. Users do not need to install Java separately.

## Windows installation

1. Download `GraphicRunnerInstallBeta.exe`.
2. Verify its SHA-256 checksum against `SHA256SUMS.txt`.
3. Run the installer and accept the beta license.
4. Because the beta is not digitally signed yet, Windows may show **Windows protected your PC**. After verifying the checksum, select **More info**, confirm the app name, and select **Run anyway**.

Do not disable Microsoft Defender or SmartScreen. Trusted code signing is the permanent fix for the unsigned-publisher warning.

## Native Linux installation

Graphic Runner v0.0.17 includes native x64 Linux builds produced and tested on an Ubuntu 22.04 baseline. Wine and Bottles are no longer required.

### Ubuntu/Debian package

Download `graphicrunner_0.0.17-1_amd64.deb`, verify its checksum, then run:

```bash
sudo apt install ./graphicrunner_0.0.17-1_amd64.deb
```

Launch **GraphicRunner** from the desktop application menu.

### Portable Linux bundle

Download `GraphicRunner-Linux-x64-0.0.17.tar.gz`, verify it, then run:

```bash
tar -xzf GraphicRunner-Linux-x64-0.0.17.tar.gz
./GraphicRunner/bin/GraphicRunner
```

The portable bundle includes its own runtime but still needs a graphical Linux desktop and standard X11/font libraries. The older Wine/Bottles route remains an optional fallback for unsupported distributions.

## Verify your download

For Graphic Runner v0.0.17 Java Beta:

```text
79DEF8B878C8DF3B6FDA8C77773C4DFA4311B3818A88A81B3EF6245A4349F7C1  GraphicRunnerInstallBeta.exe
4F686E2E7FB04B5FEBB3634EF3B72F77CAD7D8A1A9B6E05F7B0D8EFDBD219CC0  GraphicRunnerInstallBeta.msi
1AECBF89E2EA73702A7178245CD41874539CEF062A47C10483665E16F1413AAB  graphicrunner_0.0.17-1_amd64.deb
67911A8E0D05C69FD60AC1918184D4CCFABBC90C1C1FEC4BF3CBE32F94FC6621  GraphicRunner-Linux-x64-0.0.17.tar.gz
```

On Windows:

```powershell
Get-FileHash .\GraphicRunnerInstallBeta.exe -Algorithm SHA256
```

On Linux:

```bash
sha256sum graphicrunner_0.0.17-1_amd64.deb
```

## Privacy and source protection

Graphic Runner operates locally and does not upload your artwork. This public repository contains only the website, user-facing documentation, and compiled release downloads. Application source code and private build files are not included.

## Acceptable use

Each installer includes `README_FIRST.txt`, `LICENSE.txt`, the EULA v2.1 presented for acceptance, and `THIRD-PARTY-NOTICES.txt`. Users are responsible for their content and must have the rights required for every image, font, logo, trademark, and other item they use. Users may share the official release link but may not redistribute, sell, rebrand, relabel, host, or pass off Graphic Runner as their own application.

## Support

Send product feedback through the [Graphic Runner Beta Feedback form](https://forms.gle/xRCnM3ARTG7ps8CYA).

Security reports and private feedback: `taskmaster@trunner.net`

© 2026 Patrick Jamison. All rights reserved.
