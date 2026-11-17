VIRTUAL CINEMATOGRAPHER V24 — SHADOW INITIALIZATION FIX

Based on V23. All previous features are retained.

V24 fix:
- Moved the initial renderApplyQuality() call until after renderShadowMapSize is initialized and the function declaration is evaluated.
- V23 called renderApplyQuality() immediately after creating the key light, before the later let declaration of renderShadowMapSize. This caused a temporal-dead-zone ReferenceError and stopped scene initialization.
- Soft and High both use PCFShadowMap. Soft = 1024²; High = 2048².

Install:
Replace index.html and README.txt in the GitHub Pages repository root, commit, wait for deployment, then Ctrl+F5.
Do not upload check.mjs. Keep .nojekyll.
External CDN access is required.

Validation: ZIP integrity and JavaScript syntax checked. Not browser-tested on your device.
