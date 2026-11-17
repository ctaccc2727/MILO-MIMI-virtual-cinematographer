VIRTUAL CINEMATOGRAPHER V27 — MATERIAL PRESET TEXTURES

Based on V25. All prior features retained.

V27 improves the visible distinction between presets:
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


V27 FIX: Preset application now clones the original material type instead of copying it into MeshPhysicalMaterial. This prevents Vector2.copy errors on materials that do not expose physical-material properties. Clearcoat and sheen are applied only when supported by the cloned material.
