VIRTUAL CINEMATOGRAPHER V21 — SCENE RESTORE FIX

Based on V20. Retains all prior features:
- Environment Studio and imported 3D models
- Character Animation Studio and Custom Timeline
- Motion Studio and Root Motion
- Cinematic Sequencer
- Complete Project ZIP save/load
- Render Studio WebM recording and quality profiles
- V20 real-time shadows and color processing

V21 fix:
- Corrected initialization order for the V20 render quality engine.
- Initial shadow/color settings are now applied only after the scene and key light exist.
- Prevents an early JavaScript reference error from stopping 3D scene initialization.

Install:
1. Extract this ZIP.
2. Replace index.html and README.txt in the root of your GitHub Pages repository.
3. Commit changes and wait for deployment.
4. Refresh with Ctrl+F5.

Do not upload check.mjs. Keep .nojekyll.
External CDN access is required.

Validation:
ZIP integrity and JavaScript syntax checked. This build has not been browser-tested on your device.
