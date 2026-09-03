# Graphic Runner v0.0.22.4 Beta

## Pattern, workspace, and export update

- Pattern Maker supports Grid, Brick, Half-drop, and Mirror with editable area handles and a live master layer.
- Optional **Fill Area · Auto Repeat** adds repetitions as motifs shrink; manual rows and columns support up to 100 each.
- Clicking visible repeated artwork selects its owning layer; transparent gaps can select artwork underneath.
- **Runner Express** offers a simpler workspace alongside Advanced Runner. Switching workspaces preserves document capabilities and artwork.
- Narrow typography controls fit the left panel, including exact numeric values, writing direction, and font controls.
- Improved searchable font controls, previews, installed-font refresh, and vertical text.
- Improved undo/redo stability and completed-gesture history, including pattern and finishing adjustments.
- Command search is navigation-only and better protects text entry from canvas shortcuts.
- Project startup and export share dimension presets and orientation choices. Image export offers exact pixels, a pre-save preview, and encoded file size.
- Successful image export shows **Export Complete** with **Open Folder**.
- Adaptive preview rendering, pattern caching, and retained diagnostic lifecycle events support smoother editing and troubleshooting.

## Downloads

- Windows x64: `GraphicRunner-0.0.22.4-Windows-Setup.exe`
- Linux x64 DEB: `graphicrunner_0.0.22.4-1_amd64.deb`
- Linux x64 portable: `GraphicRunner-Linux-x64-0.0.22.4.tar.gz`
- Integrity checks: `SHA256SUMS_v0.0.22.4.txt`

Both platforms include a Java runtime and offline AI models; a separate Java installation is not required.

## Linux installation

For Ubuntu 22.04 or newer, install the DEB with APT so desktop dependencies are resolved:

```sh
sudo apt install ./graphicrunner_0.0.22.4-1_amd64.deb
```

The portable archive needs the same system desktop libraries. Native AI upscaling additionally needs Vulkan/OpenMP support and a compatible Vulkan device/driver; these are optional for the core editor. GPU upscaling is not guaranteed on every Linux system.

The Linux runtime uses checksum-verified Eclipse Temurin 17.0.20.1 rather than a host-specific Ubuntu JDK. Desktop dependencies include font configuration/fonts, X11, audio, and GTK (including modern t64 package alternatives).

## Verification

- Windows packaged-launcher self-tests and real bundled SAM 2/LaMa inference passed.
- Linux DEB and portable archives passed full packaged self-tests on Ubuntu 22.04 and 26.04.
- Both Ubuntu versions passed native-library audits (including bundled ONNX libraries), APT dependency resolution, and real bundled SAM 2/LaMa inference.
- Actual DEB install, installed-launcher self-test, isolated Xvfb GUI startup, and removal passed on both Ubuntu versions.
- GUI smoke checks verify startup, not every interactive editing workflow or every GPU/driver configuration.

## Beta notes

Keep backups of your projects and verify important exports. This beta is not a guarantee of fault-free editing. The previously reported Pattern Maker project wipe remains unconfirmed and was not reproduced in subsequent tests; it is not claimed as definitively fixed.

The Windows installer is not digitally signed. Verify the published SHA-256 checksum before running it. Downloads contain application binaries, runtime, models, and notices—not private source/build files.
