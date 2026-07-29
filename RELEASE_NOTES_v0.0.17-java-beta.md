# Graphic Runner v0.0.17 Java Beta

This release expands the fast Java desktop build and adds the first native
Linux packages. The application remains proprietary freeware: this public
repository and its release contain compiled downloads and user documentation,
not application source code.

## Highlights

- Undo and Redo keep the active layer, valid vector/Type Lab selection,
  editing tool, and canvas selection.
- Long layer stacks keep their scroll position when selecting a layer.
- **Merge All** flattens visible design layers at full canvas resolution or
  combines visible Logo Vector paths into one editable vector layer.
- Text, Image, Symbols, and Type Lab share a persistent design canvas.
- Logo Vector remains a separate path-only workspace with editable SVG export.
- Image mode includes stretchable solid planes.
- Export includes Camera Raw-style sharpening, clarity, tonal, brightness,
  contrast, saturation, temperature, and tint finishing controls.

## Windows

Use `GraphicRunnerInstallBeta.exe` (recommended) or
`GraphicRunnerInstallBeta.msi`. The Java runtime is included.

The Windows packages are not digitally signed yet. SmartScreen may show
**Windows protected your PC**. Verify the checksum, choose **More info**,
confirm the application name, and select **Run anyway**. Do not disable
Microsoft Defender or SmartScreen.

## Native Linux

- `graphicrunner_0.0.17-1_amd64.deb` is the native Ubuntu/Debian x64 package.
- `GraphicRunner-Linux-x64-0.0.17.tar.gz` is the portable native x64 bundle.

Both include their own Java runtime and were built and tested on an Ubuntu
22.04 baseline. Wine and Bottles are no longer required.

Install the `.deb` with:

```bash
sudo apt install ./graphicrunner_0.0.17-1_amd64.deb
```

Or unpack and run the portable build:

```bash
tar -xzf GraphicRunner-Linux-x64-0.0.17.tar.gz
./GraphicRunner/bin/GraphicRunner
```

## SHA-256

```text
79DEF8B878C8DF3B6FDA8C77773C4DFA4311B3818A88A81B3EF6245A4349F7C1  GraphicRunnerInstallBeta.exe
4F686E2E7FB04B5FEBB3634EF3B72F77CAD7D8A1A9B6E05F7B0D8EFDBD219CC0  GraphicRunnerInstallBeta.msi
1AECBF89E2EA73702A7178245CD41874539CEF062A47C10483665E16F1413AAB  graphicrunner_0.0.17-1_amd64.deb
67911A8E0D05C69FD60AC1918184D4CCFABBC90C1C1FEC4BF3CBE32F94FC6621  GraphicRunner-Linux-x64-0.0.17.tar.gz
```

## Source and license

Application source code and private build files are not included in this
repository or these release assets. Graphic Runner is proprietary freeware
licensed under the bundled EULA v2.1.
