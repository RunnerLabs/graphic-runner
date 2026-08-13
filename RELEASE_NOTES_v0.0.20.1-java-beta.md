# Graphic Runner v0.0.20.1 Java Beta

Version 0.0.20.1 is an updated offline editing release for Windows and native
Linux.

## Highlights

- Speed Form, Select, Paint, Erase, Smudge, and Clone now switch exclusively,
  preventing multiple canvas tools from running at the same time.
- Runner Developer provides final image controls for sharpening, denoise,
  color denoise, clarity, brightness, contrast, highlights, shadows,
  saturation, temperature, tint, noise, and vignette.
- AI-enhanced object selection, local inpainting, and 2x, 3x, or 4x image
  upscaling.
- A dedicated Image-mode Paint Color eyedropper samples visible canvas colors.
- Independent artboards, separate layer stacks, layout tools, cropping,
  direct image handles, clipping, locking, gradients, strokes, fill tools,
  trace rulers, and expanded dithering.
- Print True 4000 px preview, local performance diagnostics, high-quality
  export, and bundled runtimes for Windows and Linux.
- AI Edit remains withheld from this release while it receives more testing.

## Downloads

- `GraphicRunner-0.0.20.1-Windows-Setup.exe` - recommended Windows 10/11 installer.
- `GraphicRunner-0.0.20.1-Windows-Installer.msi` - managed/silent Windows installer.
- `graphicrunner_0.0.20.1_amd64.deb` - native Ubuntu/Debian x64 installer.
- `GraphicRunner-Linux-x64-0.0.20.1.tar.gz` - portable native Linux x64 bundle.
- `SHA256SUMS_v0.0.20.1.txt` - checksum manifest.

Every build includes its Java runtime and the files required for offline
editing. Wine and Bottles are not required for the Linux packages.

## SHA-256

```text
304327236A1F30A41FDFDC86FEA339A3878230F43F201D1E8F97FC728232D053  GraphicRunner-0.0.20.1-Windows-Setup.exe
56ACCD65FDF64963360D761BA8240653DC5AB27E45EBF67A68FF506F3CC244DE  GraphicRunner-0.0.20.1-Windows-Installer.msi
D54DA499983E0335E8328D7CBCFDAE66A45F118EC55D1EE6E063D342341A347C  graphicrunner_0.0.20.1_amd64.deb
51B3AD2A6CFBE2772A48BFEBFFA8AA79995EF6499108378B8F46E8BAFA19E2B9  GraphicRunner-Linux-x64-0.0.20.1.tar.gz
```

## Verification

- Full application self-test: PASS.
- Windows MSI validation and administrative extraction: PASS.
- Native Linux packaged-launcher self-test: PASS.
- Required third-party notices and licenses: present.
- Java source or class files in public packages: none.

The Windows beta is not yet digitally signed and may display a SmartScreen
unknown-publisher warning. Verify the checksum, use only the official release,
and do not disable Defender or SmartScreen.

Graphic Runner processes artwork locally. It does not upload artwork, use a
remote AI service, train on user content, or collect personal data through its
AI-enhanced tools. Complete license and third-party notices are included in
each package.
