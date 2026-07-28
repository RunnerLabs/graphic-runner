# Graphic Runner v0.0.14 Java Beta

This release returns Graphic Runner's public beta to the faster Java desktop build and publishes source-free installers for Windows. Linux users can run the same installer through the tested Wine + Bottles compatibility route.

## Highlights

- Paint and Smudge are available in Text, Image, Logo Vector, Symbols, and Type Lab.
- Smudge can pull visible pixels beyond an image or artwork boundary into transparent canvas space.
- Per-layer canvas paint survives undo, layer copy/paste, and export.
- Ember-only navigation tabs remove the old pale system-selection frame.
- Layer masks, blend modes, image import/upscale, vector manipulation, Type Lab, dithering, CRT controls, rulers, guides, and PNG/JPEG/SVG/GIF/TIFF export remain included.
- The official release link embedded in the app and installer documentation now points to RunnerLabs.

## Windows

Download `GraphicRunnerInstallBeta.exe` (recommended) or `GraphicRunnerInstallBeta.msi`. The packaged runtime is included; users do not need to install Java.

The installers are not digitally signed yet. Windows may show **Windows protected your PC**. Verify the checksum, select **More info**, confirm the application name, and then select **Run anyway**. Do not disable Microsoft Defender or SmartScreen.

## Linux

This release does not contain a native Linux binary. It has been tested by installing the Windows EXE through Wine and Bottles:

1. Create an **Application** bottle.
2. Choose **Run Executable** and select `GraphicRunnerInstallBeta.exe`.
3. Complete installation and launch Graphic Runner inside that bottle.

Plain Wine users can run `wine GraphicRunnerInstallBeta.exe`.

## SHA-256

```text
E6E7F482BAFC9FA1BFD0DCA251F0F2498D17BF8713C770E2535BDE951E8CF458  GraphicRunnerInstallBeta.exe
C33632E1C28879E04AF3D2B128655B5A22F168D1EA2463A0A637DB42CFEB2BF2  GraphicRunnerInstallBeta.msi
```

## Source and license

Application source code and private build files are not included in this repository or these release assets. Graphic Runner is proprietary freeware licensed under the bundled EULA v2.1.

Feedback: https://forms.gle/xRCnM3ARTG7ps8CYA
