# Graphic Runner v0.0.23.2 BETA

Emergency multi-artboard paint and layer-panel hotfix for Windows.

## Fixed

- Painting works on the active artboard across multi-artboard documents.
- Blank newly created artboards accept brush input before their first preview frame renders.
- Brush coordinates map to the selected artboard's local crop.
- Switching artboards keeps the active paint tool and current tab available.
- The Layers panel immediately refreshes with the selected artboard's independent layer stack.
- Collapsed layer-row state no longer leaks between artboard documents.

## Download

- Windows 10/11 x64: `GraphicRunner-0.0.23.2-Windows-Setup.exe`
- SHA-256: `E4766D2B8FA81CCC43B494D24019976240FDBB04F6A2409FE7298819D514239F`

Linux installers remain on v0.0.23.

## Verification

- Java 17-target compilation passed.
- The full source JAR self-test passed.
- New regression coverage verifies four blank artboards, immediate brush-coordinate mapping, active-document ownership, visible layer rows, and paint-tool retention.

Graphic Runner is an unsigned public beta. Verify the checksum before installing. Windows may show a publisher notice.
