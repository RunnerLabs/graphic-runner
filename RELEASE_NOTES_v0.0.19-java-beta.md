# Graphic Runner v0.0.19 Java Beta

This Windows and native Linux release sharpens Graphic Runner's everyday editing workflow while
keeping the application offline, source-private, and free to use under its
bundled license.

## Preview and finishing

- Choose Standard, High, or Ultra canvas-preview quality in Settings.
- Camera Raw adds sharpen, clarity, brightness, tone controls, color grading,
  luminance denoise, and color denoise for final export adjustments.
- The transparent alpha canvas is now borderless and easier to inspect.
- A universal black-and-white filter is available across artwork modes.

## Layout and canvas workflow

- Align layers horizontally or vertically.
- Rotate artwork in 90-degree steps and flip it horizontally or vertically.
- Create, show, hide, select, and delete optional layout artboards without
  adding them to the final export.
- Layout controls now live in their own dock panel.
- Drag image files onto the canvas or paste copied image pixels with `Ctrl+V`.

## Editing improvements

- Paint strokes preview smoothly without repeatedly multiplying their opacity.
- Press `B` to activate the paint brush.
- New blank layers are inserted beneath existing artwork for a clearer stack.
- Long operations display the delayed ember hourglass and lock editing once the
  loading overlay appears, preventing changes in the middle of AI processing.
- The splash screen links to the installed README and support page.

## Windows downloads

- `GraphicRunnerInstallBeta.exe` — recommended installer.
- `GraphicRunnerInstallBeta.msi` — alternate MSI for managed installation.

Java and the offline Real-ESRGAN models are bundled. The installers remain
unsigned, so Windows SmartScreen may show an unknown-publisher warning. Verify
the checksum, choose **More info**, confirm the application name, and then
select **Run anyway**. Do not disable Microsoft Defender or SmartScreen.

## Linux downloads

- `graphicrunner_0.0.19_amd64.deb` — native Ubuntu/Debian x64 package.
- `GraphicRunner-Linux-x64-0.0.19.tar.gz` — portable native Linux x64 bundle.

Both Linux packages include Java and the offline Real-ESRGAN models. The DEB
declares `libvulkan1`; portable users need `libvulkan1` and a current
Vulkan-capable graphics driver for AI upscale. Wine and Bottles are not needed.

## SHA-256

```text
2E962CD69B94C71E910D6D4736E3E53BD3E8A7DDD942C82CAE2CDC45A82797B0  GraphicRunnerInstallBeta.exe
D6E48DDAABF9C3787FE2525E443DBA8D8E76A63DA46545D7434C09C29360AA4C  GraphicRunnerInstallBeta.msi
86F2F540DAE922B000DF635F9F9E6B70D7F04D3C45D205548E51683A8FB7EC80  graphicrunner_0.0.19_amd64.deb
4946E8795377CA9FA31CAD051CDB82BFDC82D03705E92B3C7DA55256B468FF8B  GraphicRunner-Linux-x64-0.0.19.tar.gz
```

## Source and privacy

Graphic Runner performs editing and AI upscaling locally. The public repository
and release contain only the website, user documentation, and compiled release
downloads. Application source code and private build files are not included.
