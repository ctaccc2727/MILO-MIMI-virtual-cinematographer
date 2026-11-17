VIRTUAL CINEMATOGRAPHER V26 — MATERIAL PRESET TEXTURES

Based on V25. All prior features retained.

V26 improves the visible distinction between presets:
- Plastic: physical clearcoat highlights plus subtle surface map.
- Rubber: dark fine-grain procedural surface map and high roughness.
- Wood: procedural wood-grain color map.
- Fabric: woven crosshatch procedural color map and sheen.
- Presets are applied to all meshes under the selected object.
- Selected preset name is stored in editable primitive Scene JSON and reapplied when loading.
- Existing roughness, metalness, opacity sliders remain available.

Notes:
- Procedural maps are generated in the browser at runtime; no external texture downloads.
- Wood/Fabric appearance depends on the model's UV coordinates. Meshes without usable UVs may show limited texture detail.
- These are procedural stylized surface maps, not scanned photoreal materials.
- GLB export includes the live material maps and properties.

Install:
Replace index.html and README.txt in GitHub Pages root, commit, then Ctrl+F5.
Do not upload check.mjs. Keep .nojekyll.

Validation: ZIP integrity and JavaScript syntax checked. Not browser-tested on your device.
