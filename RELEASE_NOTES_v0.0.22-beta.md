# Graphic Runner v0.0.22 Beta

## Creative Control Update

Graphic Runner v0.0.22 is a source-free public beta for Windows 10/11 and
Ubuntu/Debian x64. The application, AI inference, and artwork processing remain
local and offline.

### Workspace and layers

- Drag any named `// TOOL` section between tabs or reorder it in place.
- Settings > UI Manager provides a compact whole-workspace view for moving,
  ordering, hiding, restoring, and resetting tools without tab shuffling.
- Panel relocation preserves the current scroll position.
- Layer masks have visible black-and-white thumbnails.
- Group/ungroup (`Ctrl+G` / `Ctrl+Shift+G`), collapsible nested layers,
  right-click Unnest, and drag-out unnesting add structured layer control.
- Solid planes are created on new layers to prevent accidental destruction.
- Image is the default workspace and the first default layer is an Image layer.

### Selection, paint, and canvas control

- `S` activates Polygon Selection, with corrected multi-corner closing.
- `G` activates Paint Bucket for filling inside or outside a selection.
- Painting inside a selection is now recorded as an atomic Undo action.
- Blank Canvas clears stale pasted images and paint buffers.
- Maximum canvas zoom is substantially higher for pixel-level editing.
- Image transform borders fit the artwork more closely; rotation and movement
  are safer and more responsive.

### Sketch Trace and editable vectors

- Stroke Trace recovers smooth centerlines instead of pixel-width silhouettes.
- Geometry Trace favors straight, sharp construction and logo lines.
- Fill Trace preserves closed silhouettes.
- Image Trace converts clean black-and-white PNG illustration art into editable
  curves while preserving filled blacks and interior white openings.
- Local AI Auto Polish uses the hash-verified MIT TEED model without uploading
  artwork, then reconnects, simplifies, and smooths the detected linework.
- Auto Polish now normalizes AI confidence bands before vector expansion, so
  fine source marks no longer become excessively thick.
- Marquee-select vector nodes, distinguish selected orange nodes from white
  unselected nodes, delete the selection together, or drag any selected node to
  move the entire selected set.

### Export, animation, and DTF

- Export Runner uses checked layers as the exact animation-preview scope while
  unchecked layers remain static.
- GIF previews default to off; individual animated layers can be previewed and
  exported, and GIF duration is capped at five seconds.
- The panel name is consistently singular: Export Runner.
- DTF has a direct threshold slider and an independent output swatch.
- Primary Paint, Plane, and regular creation-color controls remain synchronized;
  Secondary and DTF colors remain independent. White is the creation default.

### Additional quality-of-life work

- Modern social, story/video, screen, mobile, and print canvas templates.
- Noise is available in Effects with contextual controls.
- Text selection boxes can unlock dimensions for independent reshaping.
- Layer rows, Size controls, text-lock labels, and dock boundaries are corrected
  for compact and zoomed interfaces.
- Full package tests pass on the Windows and Linux payloads.

## Downloads

- `GraphicRunner-0.0.22-Windows-Setup.exe`
- `GraphicRunner-0.0.22-Windows-Installer.msi`
- `graphicrunner_0.0.22_amd64.deb`
- `GraphicRunner-Linux-x64-0.0.22.tar.gz`
- `SHA256SUMS_v0.0.22.txt`

The Windows beta is not digitally signed yet, so SmartScreen may show an
unknown-publisher warning. Verify the published checksum before running it.
The Linux DEB declares its desktop, Vulkan, and OpenMP runtime dependencies.

Application source code and private build files are not included.
