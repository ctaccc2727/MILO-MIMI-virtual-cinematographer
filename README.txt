VIRTUAL CINEMATOGRAPHER V20 — CINEMATIC RENDER ENGINE

Based on V19. All previous features are retained.

V20 adds:
- Real-time directional-light shadows: Off, Soft (1024²), High (2048²).
- Shadow casting and receiving for scene meshes when rendering starts or controls change.
- Color processing: ACES Filmic, Neutral, Linear.
- Texture anisotropic filtering up to the device/GPU-supported maximum.
- Existing WebGL antialiasing remains enabled.

Limitations:
- Real-time WebGL rendering, not offline/path-traced rendering.
- Shadow maps use the main directional/key light only.
- High shadow resolution can reduce performance, especially on tablets.
- Check the image after changing tone mapping; it changes the overall look.
- No ray tracing, denoising, offline rendering, or multi-bounce global illumination.

Install by replacing index.html and README.txt in the GitHub Pages repository, commit, then refresh with Ctrl+F5.
Do not upload check.mjs. Keep .nojekyll.
External CDN access is required.

Validation: ZIP integrity and JavaScript syntax checked. Not browser-tested on your device.
