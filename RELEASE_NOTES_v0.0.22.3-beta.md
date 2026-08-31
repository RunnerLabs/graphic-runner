# Graphic Runner v0.0.22.3 Beta

## Creative Control Update

This release extends the Creative Control Update with a sharper vector-first
workflow, more flexible workspace organization, performance improvements, and
tester-driven fixes. Graphic Runner and its AI tools remain local and offline.

### Vector, perspective, and layout

- Logo Vector is now named **Vector** throughout the interface.
- Live text converts directly from font outlines into clean editable curves,
  preserving straight edges and compound letter shapes without bitmap tracing.
- Four-corner Perspective works non-destructively on image, live text, symbols,
  and vector geometry. `Shift+P` opens the editor for a supported layer.
- Vector mode can create editable background planes using the complete set of
  Image canvas templates, reducing unnecessary workspace handoffs.
- Layer context menus expose eligible Rasterize, Convert to Curves, and
  Perspective actions.

### Workspace and visual comfort

- Right-side tabs can be reordered by dragging or detached into individual
  floating toolbars so several panels can remain visible together.
- Tab clicking, hover cursors, drag feedback, and theme switching were repaired.
- Added the Task and neutral Dark Gray themes, plus a persistent UI-only
  blue-light filter that never changes canvas colors or exported artwork.
- Composition overlays can rotate, Effects can be searched, and the misplaced
  Canvas `+FONT` control was removed.

### Editing and performance

- Speed Form nodes now follow the pointer through an immediate overlay and
  commit one final full render on release.
- Render scheduling cancels obsolete work and bounds interactive High/Ultra
  previews before the final full-quality result.
- Mock Runner grids can be moved from their interior. Cylinder grids support
  editable profile nodes, stronger center curvature, and edge compression.
- Gradient reversal is functional and undoable. Stroke controls are now
  context-specific for raster, vector, and live text/shape workflows.

### Reliability and Linux

- Offline AI Object Selection now preserves its inference source and prompt
  markers while the local SAM 2 model runs.
- Linux browser clipboard support accepts native PNG stream flavors in addition
  to Java image data.
- Direct text color and authored Effects now use clear mutually exclusive states.
- The native Linux package uses a controlled dependency list so optional Vulkan
  and OpenMP support cannot block the main editor installation.

### Release verification

- Windows Setup passed a silent native install and the complete packaged self-test.
- The Linux DEB passed checksum and metadata checks, a 26-file ELF dependency
  audit, APT dependency simulation, an actual install/launch/remove cycle on
  Ubuntu 22.04, cross-version launch checks, and real bundled AI inference.

## Downloads

- `GraphicRunner-0.0.22.3-Windows-Setup.exe`
- `graphicrunner_0.0.22.3-2_amd64.deb`
- `GraphicRunner-Linux-x64-0.0.22.3.tar.gz`
- `SHA256SUMS_v0.0.22.3.txt`

The Windows beta is not digitally signed yet. Verify the published SHA-256
checksum before running it. Application source and private build files are not
included in these downloads.
