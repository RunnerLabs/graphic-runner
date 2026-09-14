# Graphic Runner v0.0.23.1 BETA

Artboard and masking reliability hotfix for Windows.

## Artboards and layers

- Layers, solid planes, images, vectors, and text are created on the active artboard.
- Switching artboards preserves each document's layers, workspace position, and local crop.
- Artboards with equal pixel dimensions now display at equal workspace sizes.
- The new-artboard dialog supports presets or custom dimensions, portrait or landscape orientation, and batches of 1-20 artboards.

## Masks and selections

- Selection outlines can be hidden without clearing the live selection, making edge refinement easier to inspect.
- Feather, Edge, and Smooth update attached masks while controls move, then settle at full quality on release.
- Mask rows display their source layer and provide a Source action to restore source-layer selection.
- Invalid or orphaned active-mask references recover during layer-list refresh instead of trapping layer controls.

## Download

- Windows 10/11 x64: `GraphicRunner-0.0.23.1-Windows-Setup.exe`
- SHA-256: `47B54F21346A7C24CF3933C4284CFC3D62E9864FD04D99E262E8A5A86F86E435`

Linux installers remain on v0.0.23 and are available from the [v0.0.23 release](https://github.com/RunnerLabs/graphic-runner/releases/tag/v0.0.23).

## Verification

- Java 17-target compilation passed.
- The packaged release JAR passed the complete built-in self-test: 91 checks and `SELFTEST PASS`.
- Regression coverage verifies two independent 1080 x 1350 artboards, equal display sizing, active-artboard plane creation, retained workspace positions, and distinct per-artboard preview pixels.
- The installer includes its Java runtime, offline AI models, notices, security information, and user documentation.

Graphic Runner is an unsigned public beta. Verify the checksum before installing. Windows may show a publisher notice.
