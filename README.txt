VIRTUAL CINEMATOGRAPHER V8 — ANIMATION TIMELINE STUDIO

V8 continues from V7 and retains the adaptive desktop/tablet interface, camera controls,
lens and depth of field, lighting studio, environment editor, GLB/GLTF import,
embedded animation playback, and skeleton inspector.

New explicit interface layout switch:
- Header selector: Auto layout / Desktop / Tablet.
- Auto follows the browser screen and input device; Desktop and Tablet can be forced manually.

New custom animation timeline:
- Capture the current local quaternion pose of every detected bone as a keyframe.
- Add a keyframe at the current timeline time; update a keyframe at that time.
- Scrub the custom timeline and select keyframes from the list.
- Play custom animation with quaternion spherical interpolation (SLERP) between poses.
- Stop, delete, and duplicate selected keyframes.
- Set clip duration (1–30 seconds) and frame rate (24/25/30/60 fps).
- Save/load a reusable animation project JSON.

How to use:
1. Import a rigged GLB character.
2. Stop any embedded animation clip.
3. Set time to 0, pose bones with Skeleton Inspector and click Add keyframe.
4. Move the custom timeline to a later time, change bone rotations, click Add keyframe.
5. Add at least two keyframes and click Play custom.
6. Save animation JSON to keep the project.

Important limitations:
- Keyframes capture local bone rotations (quaternions), not mesh/object transforms or root motion.
- The project JSON is matched to the character's bone order and names; load it with the same compatible character rig.
- This version does not bake the custom timeline into a new GLB/GLTF file or export a standard animation clip.
- The imported clip player and custom timeline are separate modes.
- Performance depends on model complexity and device GPU.
- Three.js and GLTFLoader load from jsDelivr CDN; internet access is required.

GitHub Pages update:
1. Extract this ZIP.
2. Open the repository root.
3. Add file -> Upload files.
4. Upload index.html and README.txt, replacing existing versions.
5. Commit changes. Keep .nojekyll unchanged.
6. GitHub Pages rebuilds from main / root automatically.
