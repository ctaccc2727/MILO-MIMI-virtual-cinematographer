VIRTUAL CINEMATOGRAPHER V7 — CHARACTER ANIMATION STUDIO

V7 continues from V6 and retains the adaptive desktop/tablet interface, camera controls,
lens/DOF, lighting studio, and environment object editor.

New Character Animation Studio:
- Import rigged GLB/GLTF characters.
- Read animation clips embedded in the imported glTF.
- Select a character and animation clip.
- Play, pause, stop, and scrub the clip timeline.
- Playback speed control from 0.1x to 2.0x.
- Skeleton inspector with detected bone list.
- Manual preview rotation of a selected bone and reset to its captured local quaternion.
- The Environment Studio importer also registers imported clips for playback.

Important limitations:
- Imported model must contain a compatible skeleton for bone inspection.
- Playback only plays clips embedded in the GLB/GLTF; it does not generate new motion.
- Manual bone rotation is a preview adjustment; playing a clip may overwrite it.
- This version does not yet author keyframes, retarget motion capture, or export edited animations.
- Self-contained GLB is recommended. GLTF files with external dependencies may fail when only one file is selected.
- Three.js and GLTFLoader load from jsDelivr CDN; internet access is required.
- Designed for desktop and tablet responsive layouts; test large rigs against device GPU.

GitHub Pages update:
1. Extract this ZIP.
2. Open the repository root.
3. Add file -> Upload files.
4. Upload the new index.html and README.txt, replacing existing versions.
5. Commit changes. Keep .nojekyll unchanged.
6. GitHub Pages rebuilds from main / root automatically.

Netlify is not required.
