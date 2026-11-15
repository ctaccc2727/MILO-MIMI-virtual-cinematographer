VIRTUAL CINEMATOGRAPHER V5 — LIGHTING STUDIO

V5 continues from the working V4.3 DOF FIX build. It preserves the camera modes,
desktop controls, tablet touch controls, lens/sensor settings, and Depth of Field.

New Lighting Studio:
- Main/key directional light: intensity, color temperature (2000K–10000K), and XYZ position.
- Fill directional light: intensity and color.
- Hemisphere/ambient light: intensity.
- Rim point light: intensity and color.
- Environment background color.
- Fog ON/OFF and fog distance.
- Tone-mapping exposure.
- Daylight, Warm Interior, and Night/Moonlight presets.
- Save/load lighting preset JSON.
- Camera preset JSON now also includes lighting settings.

Known limitations:
- This stage does not yet include HDRI image loading, physically based area lights,
  shadow-map controls, or a full light-gizmo editor. Those are planned for later stages.
- The lighting rig is a practical real-time preview setup, not a physically calibrated
  film-set photometric simulator.
- Three.js and post-processing modules load from jsDelivr CDN; internet access is required.

GitHub Pages update:
1. Open the repository root.
2. Add file -> Upload files.
3. Upload the new index.html and README.txt from this package, replacing the existing files.
4. Commit changes. Keep .nojekyll unchanged.
5. GitHub Pages automatically rebuilds from main / root.

Netlify is not required for this deployment.
