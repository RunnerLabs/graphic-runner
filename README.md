# Graphic Runner

Graphic Runner is a free offline desktop graphics studio for creating high-impact text, image, logo-vector, symbol, and print effects. The public beta is proprietary freeware, not open-source software.

## Download

Download the latest build from the [official GitHub release](https://github.com/RunnerLabs/graphic-runner/releases/latest).

- `GraphicRunnerInstallBeta.exe` — recommended Windows 10/11 installer.
- `GraphicRunnerInstallBeta.msi` — alternate Windows MSI installer.
- `SHA256SUMS.txt` — checksums for verifying both installers.

The installer includes Graphic Runner's Java runtime. Users do not need to install Java separately.

## Windows installation

1. Download `GraphicRunnerInstallBeta.exe`.
2. Verify its SHA-256 checksum against `SHA256SUMS.txt`.
3. Run the installer and accept the beta license.
4. Because the beta is not digitally signed yet, Windows may show **Windows protected your PC**. After verifying the checksum, select **More info**, confirm the app name, and select **Run anyway**.

Do not disable Microsoft Defender or SmartScreen. Trusted code signing is the permanent fix for the unsigned-publisher warning.

## Linux installation — Wine + Bottles

Graphic Runner v0.0.14 is a Windows desktop build. It has been tested on Linux through Wine and Bottles; this release does not include a native Linux binary.

### Bottles

1. Install [Bottles](https://usebottles.com/) and create an **Application** bottle.
2. Download `GraphicRunnerInstallBeta.exe` from the latest Graphic Runner release.
3. In Bottles, open the bottle, choose **Run Executable**, and select the installer.
4. Complete the installer and launch Graphic Runner from that bottle.

### Plain Wine

With Wine installed, run:

```bash
wine GraphicRunnerInstallBeta.exe
```

Linux compatibility depends on the installed Wine/Bottles version, graphics drivers, and desktop environment. If one runner has a display issue, try the current Bottles Application environment.

## Verify your download

For Graphic Runner v0.0.14 Java Beta:

```text
E6E7F482BAFC9FA1BFD0DCA251F0F2498D17BF8713C770E2535BDE951E8CF458  GraphicRunnerInstallBeta.exe
C33632E1C28879E04AF3D2B128655B5A22F168D1EA2463A0A637DB42CFEB2BF2  GraphicRunnerInstallBeta.msi
```

On Windows:

```powershell
Get-FileHash .\GraphicRunnerInstallBeta.exe -Algorithm SHA256
```

On Linux:

```bash
sha256sum GraphicRunnerInstallBeta.exe
```

## Privacy and source protection

Graphic Runner operates locally and does not upload your artwork. This public repository contains only the website, user-facing documentation, and compiled release downloads. Application source code and private build files are not included.

## Acceptable use

Each installer includes `README_FIRST.txt`, `LICENSE.txt`, the EULA v2.1 presented for acceptance, and `THIRD-PARTY-NOTICES.txt`. Users are responsible for their content and must have the rights required for every image, font, logo, trademark, and other item they use. Users may share the official release link but may not redistribute, sell, rebrand, relabel, host, or pass off Graphic Runner as their own application.

## Support

Send product feedback through the [Graphic Runner Beta Feedback form](https://forms.gle/xRCnM3ARTG7ps8CYA).

Security reports and private feedback: `taskmaster@trunner.net`

© 2026 Patrick Jamison. All rights reserved.
