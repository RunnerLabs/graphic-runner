# Graphic Runner v0.0.20 Java Beta

Version 0.0.20 is a major offline editing update for Windows and native Linux.

## Highlights

- AI-enhanced object selection with persistent edges, additive/exclusion
  prompts, feather, edge, smoothing, Auto Polish, and one-click masking.
- AI-enhanced inpainting for reconstructing selected image areas locally.
- A dedicated Image-mode Paint Color eyedropper that samples an exact visible
  canvas color without changing the separate transparency/key-color tool.
- Speed Form Mode with five tapered industrial-sketch profiles, pressure
  simulation, stabilization, and round or block marker tips.
- Independent artboards with separate layer stacks, selection, movement,
  resizing, and single or batch PNG export.
- Layer locking, faster visibility/order/blend interaction, clipping to the
  layer below, Merge All, and corrected order shortcuts.
- Direct image handles, cropping, alignment, rotation, flipping, pasting to a
  new layer, and Convert to Curves.
- Persistent rectangle, oval, freehand, polygon, color, and AI-enhanced
  selections with invert and mask actions.
- Paint, eraser, smudge, clone, flexible trace rulers, gradients, strokes,
  expanded dither/glow controls, and more themes.
- Print True 4000 px preview, Runner Developer finishing, denoise, improved
  anti-aliasing, local performance diagnostics, and high-quality export.

## Downloads

- `GraphicRunner-0.0.20-Windows-Setup.exe` - recommended Windows 10/11 installer.
- `GraphicRunner-0.0.20-Windows-Installer.msi` - managed/silent Windows package.
- `GraphicRunner-0.0.20-Windows-Portable.zip` - optional no-install build.
- `graphicrunner_0.0.20_amd64.deb` - native Ubuntu/Debian x64 package.
- `GraphicRunner-Linux-x64-0.0.20.tar.gz` - portable native Linux x64 bundle.
- `SHA256SUMS.txt` - checksum manifest.

Every build includes its own Java runtime and the files required for its
offline editing features. Wine and Bottles are not required for the Linux
packages.

## SHA-256

```text
7253F165CA27B7E33690A37242D0A7D13EE5886AF8A5B63BF64AA15A964BEEB0  GraphicRunner-0.0.20-Windows-Setup.exe
9BDAB03A49F773DE5FD06A23F81CF97AC755C519D58A727E917D3EDDFEC217C5  GraphicRunner-0.0.20-Windows-Installer.msi
1B57EBBA4140929950A7C96614C9106647740818CE5F6A9E7314A6324397927C  GraphicRunner-0.0.20-Windows-Portable.zip
6907D5E21C9A4A2C78CED93D76541819A21569790D521BCD15B22578B770FE21  graphicrunner_0.0.20_amd64.deb
843CC0EC94B7A880B0BE6A39C90981C49CE0290115B6539D946D6FB13EE8EC78  GraphicRunner-Linux-x64-0.0.20.tar.gz
```

## Verification

- Windows build and full application self-test: PASS.
- Native Linux build and full application self-test: PASS.
- Native Linux offline AI operation: PASS.
- Required models and third-party licenses: present.
- Source files in public packages: none.

The Windows beta is not yet digitally signed and may display a SmartScreen
unknown-publisher warning. Verify the checksum, use only the official release,
and do not disable Defender or SmartScreen.

Graphic Runner processes artwork locally. It does not upload artwork, use a
remote AI service, train on user content, or collect personal data through its
AI-enhanced tools. Complete license and third-party notices are included in
each package.
