VIRTUAL CINEMATOGRAPHER V28 — MATERIAL TEXTURE RESET

Based on V27. All previous features are retained.

V28 fixes material preset switching:
- Every preset explicitly replaces the current texture map, including clearing it for Metal, Chrome, and Glass.
- Original object/material tint is preserved and restored when switching away from procedural texture presets.
- Prevents Wood/Fabric/Rubber/Plastic texture maps from leaking into the next preset.
- Existing roughness, metalness, opacity, clearcoat, sheen, Scene JSON, and GLB export behavior are retained.

Install:
1. Extract this ZIP.
2. Replace index.html and README.txt in the GitHub Pages repository root.
3. Commit changes and wait for Pages to update.
4. Refresh the site with Ctrl+F5.

Do not upload check.mjs. Keep .nojekyll.

Validation: ZIP integrity and JavaScript syntax checked. Not browser-tested on the user's device.
