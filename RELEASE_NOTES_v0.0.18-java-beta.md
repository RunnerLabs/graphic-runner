# Graphic Runner v0.0.18 Java Beta

This release replaces the old interpolation-only upscale with genuine offline
AI enhancement while keeping Graphic Runner fast, local, and source-private.
The public repository and release contain compiled downloads and user
documentation, not application source code.

## New: offline AI upscale

- **Photo / General** uses the Real-ESRGAN x4plus model for photographs and
  mixed artwork.
- **Art / Logo** uses the illustration-focused x4plus-anime model for cleaner
  drawn edges and graphic artwork.
- Both modes offer 2x, 3x, and 4x output. The model runs at its trained 4x
  scale and Graphic Runner cleanly reduces the complete result when 2x or 3x
  is requested.
- Images are processed locally through Vulkan. Nothing is uploaded and no
  backend account is required.
- **Classic: Fast** remains available as the compatibility fallback when the
  graphics driver cannot run the AI engine.
- AI jobs use bounded 256-pixel tiles, a 64-megapixel working limit, delayed
  loading feedback, and leave the original layer unchanged if inference fails.

The bundled Real-ESRGAN models and ncnn Vulkan runner are distributed under
their upstream licenses. Full attribution and license text are included in
`THIRD-PARTY-NOTICES.txt` inside every package.

## Windows

Use `GraphicRunnerInstallBeta.exe` (recommended) or
`GraphicRunnerInstallBeta.msi`. Java and both offline AI models are included.

The packages are not digitally signed yet. SmartScreen may show **Windows
protected your PC**. Verify the checksum, choose **More info**, confirm the
application name, and select **Run anyway**. Do not disable Microsoft Defender
or SmartScreen.

## Native Linux

- `graphicrunner_0.0.18-1_amd64.deb` is the native Ubuntu/Debian x64 package.
- `GraphicRunner-Linux-x64-0.0.18.tar.gz` is the portable native x64 bundle.

Both include Java and the Linux AI engine/models. The DEB declares
`libvulkan1`; portable users need that standard Vulkan runtime and a current
Vulkan-capable Intel, AMD, or NVIDIA driver.

Install the `.deb` with:

```bash
sudo apt install ./graphicrunner_0.0.18-1_amd64.deb
```

Or unpack and run the portable build:

```bash
tar -xzf GraphicRunner-Linux-x64-0.0.18.tar.gz
./GraphicRunner/bin/GraphicRunner
```

## SHA-256

```text
F4053FD6B3DF68B664212A2CAC90DFF416510976FF39BF30835918F2567B4C09  GraphicRunnerInstallBeta.exe
08D3E32842E066A868CC147E5B89B4CE03CC85259DDD2A16AA63FB9619DC65A5  GraphicRunnerInstallBeta.msi
1F1DF51BE88B4B8291826E1B7F5EAEC9F7A2BED50048A308B79DA8D5CF741563  graphicrunner_0.0.18-1_amd64.deb
CD5477F5E0BA3C9ADD3865B7C15E94E4EA0183D15226B3244A68FF01501E59BA  GraphicRunner-Linux-x64-0.0.18.tar.gz
```

## Source and license

Application source code and private build files are not included in this
repository or these release assets. Graphic Runner is proprietary freeware
licensed under the bundled EULA v2.1.
