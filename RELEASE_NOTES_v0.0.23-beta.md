# Graphic Runner v0.0.23 BETA

Photo Runner, Contour Flow, color control, and smoother masking.

## Creative controls

- Photo Runner brings independent brightness, contrast, exposure, highlights, shadows, saturation, vibrance, warmth, tint, vignette, and finer photographic grain to Style.
- Luminance-preserving color balance and a selective HSL mixer provide more control over actual image colors.
- Signal Track adds modulated diffuse X/Y, uniform modulation, line variants, and Contour Flow. Smoothed image relief bends lines around light and shade; it is not a 3D depth reconstruction.
- Signal Track and dithering stack together. Photo Runner and HSL grade the finished patterns. Signal Color Mix defaults to source colors, with optional palette blending and transparent gaps.
- Refined line spacing gives finer control at low values and avoids oversized contour bands.
- One Main Glow section is visible and searchable in Post, with amount, halo radius, threshold, tint, and hot-core controls. Cyber Runner retains its own glow.
- Gaussian, Focus, and Speed blur can soften the finished layer or run before patterns. Preserve Alpha keeps the original opacity and silhouette.

## Editing and performance

- Crop Canvas locks and unlocks crop handles without resetting the canvas position. Fit Canvas to Image uses a single image's dimensions from the right panel.
- Pattern Maker and MASK / SELECT MASK have larger click targets. DTF preparation is available from an accessible checkbox. Live Stroke Preview starts unchecked.
- Mask previews coalesce pending requests rather than repeatedly canceling unfinished renders. Mask-only changes reuse cached effects, and mutable-mask cache keys avoid repeated-stroke collisions.
- Main Glow avoids redundant pixel work. A local synthetic contour/dither/glow benchmark measured about 88 ms per cached mask frame versus 151 ms uncached; actual performance varies by project and hardware.
- Local diagnostics retain crop/effect events and record effective spacing, mixing, alpha preservation, grading placement, and mask-cache reuse.

## Downloads and Linux dependencies

- Windows 10/11 x64: GraphicRunner-0.0.23-Windows-Setup.exe.
- Ubuntu 22.04+ x64: graphicrunner_0.0.23-1_amd64.deb. Install with `sudo apt install ./graphicrunner_0.0.23-1_amd64.deb` so dependencies are resolved.
- Linux x64 portable: GraphicRunner-Linux-x64-0.0.23.tar.gz.
- SHA256SUMS_v0.0.23.txt contains download checksums.

All packages include Java and the offline AI models. The DEB declares the required font, X11, GTK, audio, C/C++, Vulkan-loader, and OpenMP libraries, with t64 alternatives for newer Ubuntu versions. Portable users need those system libraries too. Native GPU upscaling additionally requires a compatible Vulkan device and driver; bundling the loader cannot supply a GPU driver.

## Compatibility

Existing documents can look different because Signal spacing and Photo Runner stage order changed. Documents without the new mixing controls load with source colors and Preserve Alpha enabled. Keep a copy when comparing with the preceding beta.

## Verification

- Windows packaged-launcher self-test and real bundled SAM 2 / LaMa inference passed.
- Ubuntu 22.04 and 26.04: actual DEB install, installed-launcher self-test, Xvfb GUI startup, and removal passed.
- Both Linux versions: all bundled native-library dependencies resolved, APT dependency simulation passed, and extracted DEB and portable self-tests passed.
- Real bundled SAM 2 and LaMa inference passed on both Linux versions.
- Release-JAR contour/Photo Runner/dither, alpha-preservation, mask-cache pixel-equivalence, and UI-search regressions passed.
- Release payload contains application classes and bundled native AI libraries, with no application source or QA classes.
- GUI checks cover startup; Vulkan GPU compatibility still depends on the user's hardware and driver.
