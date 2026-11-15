VIRTUAL CINEMATOGRAPHER — V13 PROJECT STUDIO

V13 extends V12 and retains all previous features:
- Camera controls, optics, depth of field and presets
- Lighting Studio and Environment Studio
- GLB/GLTF import, character animation and skeleton inspector
- Root Motion, custom pose timeline and keyframe easing
- Cinematic Sequencer
- Auto / Desktop / Tablet layouts
- V12 standalone GLB and project manifest export

NEW IN V13 — COMPLETE PROJECT ARCHIVE
Use Environment Studio → Export Studio → Complete project:
1. Save complete project (.zip)
   Creates one archive containing:
   - scene.glb: complete visible stage, imported models, primitives and embedded source animation clips
   - project.json: scene metadata, camera settings, lighting, camera sequence, imported model names
   - lighting.json
   - camera-sequence.json
   - custom-animation.json when a custom pose timeline exists
2. Load complete project (.zip)
   Restores the GLB stage, camera/optics, lighting, camera sequence and custom pose timeline
   when the matching rigged character skeleton is present.

IMPORTANT
- Complete project ZIP uses JSZip loaded from jsDelivr on demand; internet access is required for this operation.
- GLB import/export uses Three.js GLTFLoader/GLTFExporter from jsDelivr.
- The ZIP contains the full stage GLB and the custom pose timeline JSON. Custom pose animation is restored as editable timeline data; it is not baked into the GLB animation tracks.
- Camera shots are restored as editable sequencer data; this is not a rendered movie.
- The project loader replaces the current stage contents. Save any current work before loading another project.
- If a custom animation skeleton does not match, the scene is restored but custom keyframes are not applied.
- This version is syntax-checked and archive-checked. Actual browser interaction and device testing must be performed in the user's browser.

INSTALL
1. Extract this ZIP.
2. Open the GitHub repository:
   https://github.com/ctaccc2727/MILO-MIMI-virtual-cinematographer
3. Add file → Upload files.
4. Upload index.html and README.txt from this V13 folder to the repository root, replacing the previous versions.
5. Commit changes, wait for GitHub Pages, then hard refresh with Ctrl+F5.
6. Do not upload this ZIP itself. Keep .nojekyll in the repository.
