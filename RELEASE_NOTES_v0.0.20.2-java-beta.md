# Graphic Runner v0.0.20.2 Java Beta

Version 0.0.20.2 is a focused stability and painting update for Windows and
native Linux.

## Highlights

- Painting inside an active selection is now substantially faster and begins
  immediately instead of appearing only after mouse release.
- Completed paint stays on the exact selected layer, including when painting
  above a separate solid-plane layer.
- Live strokes remain pinned to their intended layer through interface and
  layer refreshes.
- Selection boundaries stay available while painting until the user explicitly
  deselects them.
- Speed Form keeps its flat, anti-aliased tapered body without patterned or
  blobbed endpoints.
- The existing v0.0.20 toolset remains included: AI-enhanced local object
  selection, inpainting and upscaling; independent artboards; clipping;
  gradients; strokes; fill tools; trace rulers; Print True preview; Runner
  Developer finishing; and performance diagnostics.
- AI Edit remains withheld while it receives more testing.

## Downloads

- `GraphicRunner-0.0.20.2-Windows-Setup.exe` - Windows 10/11 per-user installer.
- `graphicrunner_0.0.20.2_amd64.deb` - native Ubuntu/Debian x64 installer.
- `GraphicRunner-Linux-x64-0.0.20.2.tar.gz` - portable native Linux x64 bundle.
- `SHA256SUMS_v0.0.20.2.txt` - checksum manifest.

Every package includes its Java runtime and the files required for offline
editing. Wine and Bottles are not required for the Linux packages.

## SHA-256

```text
6F514F7F0DA7F709400226E88596D013985C62BB141F2DAE436CB9FE12A34DB3  GraphicRunner-0.0.20.2-Windows-Setup.exe
EB244EAD75CC49686B7A02341EC4388FA17A50A8DF97009AF8AEA4F1949F1CE2  graphicrunner_0.0.20.2_amd64.deb
08701B73B46E5C56DBD535897B8D01711226168328D4378B7128139F6250FBAA  GraphicRunner-Linux-x64-0.0.20.2.tar.gz
```

## Verification

- Full Windows packaged-launcher self-test: PASS.
- Full native Linux packaged-launcher self-test: PASS.
- Focused selected-paint latency and persistence regressions: PASS.
- Required third-party notices and licenses: present.
- Source-like application files in public packages: none.

The Windows beta is not yet digitally signed and may display a SmartScreen
unknown-publisher warning. Verify the checksum, use only the official release,
and do not disable Defender or SmartScreen.

Graphic Runner processes artwork locally. It does not upload artwork, use a
remote AI service, train on user content, or collect personal data through its
AI-enhanced tools. Complete license and third-party notices are included in
each package.
