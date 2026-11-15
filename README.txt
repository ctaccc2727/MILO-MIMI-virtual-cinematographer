VIRTUAL CINEMATOGRAPHER V6 — ENVIRONMENT STUDIO

V6 continues from V5 Lighting Studio and preserves:
- Free, Cinematic, and Orbit camera modes
- Keyboard movement and on-screen touch joysticks
- Lens sensor profiles, focal length, aperture, focus distance, and DOF
- Lighting Studio controls, presets, and JSON presets

New Environment Studio:
- Add cube, sphere, cylinder, and plane primitives.
- Import GLB / GLTF models through Three.js GLTFLoader.
- Select objects from the scene object list.
- Edit position X/Y/Z, rotation X/Y/Z, and uniform scale.
- Change object color for mesh materials.
- Duplicate, delete, hide/show, and reset transforms.
- Save and load scene layouts as JSON.

Important limitations:
- Scene JSON saves the editable primitive objects and their transforms/material color.
- Imported GLB/GLTF model geometry is not embedded into the JSON scene file; re-import source model files after loading a scene.
- GLTF files that depend on external texture/buffer URLs may not import from a single selected file. Self-contained GLB is recommended.
- This stage uses numeric transform controls rather than viewport transform gizmos.
- No claim of physical testing on every GLB rig or device. Validate your own models and GPU performance.

GitHub Pages update:
1. Extract this ZIP.
2. Open the repository root.
3. Add file -> Upload files.
4. Upload the new index.html and README.txt, replacing existing versions.
5. Commit changes. Keep .nojekyll.
6. GitHub Pages rebuilds from main / root automatically.

Netlify is not required.
