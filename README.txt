VIRTUAL CINEMATOGRAPHER V25 — MATERIALS STUDIO

Based on V24. All previous features are retained.

Adds Material Editor for the selected scene object:
- Roughness, metalness and opacity controls.
- Surface presets: Plastic, Rubber, Wood, Metal, Chrome, Glass, Fabric.
- Save named material entries in the current in-memory library.
- Export/import material library JSON.
- Scene JSON stores material roughness, metalness and opacity for editable primitives; older scene JSON remains supported.
- GLB export uses edited live materials.

Notes:
- Presets adjust PBR surface properties, not image texture maps. Wood/Fabric are roughness presets only.
- Material library remains in memory until exported.
- Imported GLB: changes apply to all mesh materials under selected model root.
- Glass preset uses opacity/transparency, not physically accurate refraction.

Install:
Replace index.html and README.txt in GitHub Pages root, commit, then Ctrl+F5.
Do not upload check.mjs. Keep .nojekyll. External CDN access required.

Validation: ZIP integrity and JavaScript syntax checked. Not browser-tested on your device.
