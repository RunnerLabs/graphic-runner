# Graphic Runner v0.0.19.1 Java Beta

This anti-aliasing maintenance release keeps the public v0.0.19 feature set
while making the working canvas much more closely match the final print export.
It does not include the private v0.0.20 AI object-selector work.

## Preview and image-quality improvements

- **Ultra / Print True** renders through the 400% / 4000 px print path and
  downsamples the result for display.
- Image placement and scaling preserve fractional coordinates instead of
  rounding before sampling.
- Image, mask, layer-transform, preview, and export scaling use bicubic
  interpolation with high-quality alpha and color interpolation.
- Text, vectors, strokes, and transformed artwork use consistent anti-aliasing
  and fractional metrics.
- A regression test protects diagonal image edges from hard nearest-neighbor
  stair steps.

Ultra / Print True uses more memory and render time than Standard or High.
During direct manipulation Graphic Runner may use a faster temporary preview;
the Print True result appears after the edit settles.

## Downloads

- `GraphicRunner-0.0.19.1-Windows-Portable.zip` — Windows 10/11 portable build.
- `graphicrunner_0.0.19.1_amd64.deb` — native Ubuntu/Debian x64 package.
- `GraphicRunner-Linux-x64-0.0.19.1.tar.gz` — portable native Linux x64 bundle.

Every package includes Java and the offline Real-ESRGAN upscaling components.
The Windows package is portable because local Microsoft WiX installer
validation could not complete cleanly for this maintenance build. Extract the
ZIP and run `GraphicRunner\GraphicRunner.exe`. The unsigned executable may
trigger Windows SmartScreen; verify the checksum and do not disable Defender or
SmartScreen.

## SHA-256

```text
15709E64C4002FAA359F9ED88219EA1C13EDEF198F73CD6AF36A0444FB38F15D  GraphicRunner-0.0.19.1-Windows-Portable.zip
33C7289C9324C369E3A27F4C8675FE87D424084871E6A4FE1B76E576CF4E1FE8  graphicrunner_0.0.19.1_amd64.deb
96A1531D682BB704809A8DE5364FE04DA8A454B34612011365A39E6F85F49060  GraphicRunner-Linux-x64-0.0.19.1.tar.gz
```

## Verification and privacy

- Windows packaged self-test: PASS.
- Native Linux package verification: PASS.
- Print True 4000 px preview-path regression: PASS.
- Source files in public packages: none.
- SAM2, ONNX Runtime, and v0.0.20 object-selector files: none.

Graphic Runner performs editing and AI upscaling locally. The public repository
and release contain only the website, user documentation, and compiled release
downloads. Application source code and private build files are not included.
