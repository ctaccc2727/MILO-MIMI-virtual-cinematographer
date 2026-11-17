VIRTUAL CINEMATOGRAPHER V23 — SHADOW QUALITY FIX

Based on V22. All previous studios and features are retained.

V23 fixes High shadow mode:
- Both Soft and High use the stable PCFShadowMap filter.
- Soft uses a 1024×1024 shadow map.
- High uses a 2048×2048 shadow map.
- When switching map resolution, the old GPU shadow render target is disposed and recreated at the new size.
- This avoids switching to PCFSoftShadowMap, which caused shadows to disappear on some GPU/browser combinations.

Install:
1. Extract this ZIP.
2. Replace index.html and README.txt in the GitHub Pages repository root.
3. Commit changes and wait for deployment.
4. Refresh with Ctrl+F5.

Do not upload check.mjs. Keep .nojekyll.
External CDN access is required.

Validation:
ZIP integrity and JavaScript syntax checked. Not browser-tested on your device.
