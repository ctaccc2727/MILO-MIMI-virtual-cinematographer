VIRTUAL CINEMATOGRAPHER — V12 EXPORT STUDIO

V12 extends V11 and retains all previous modules: camera and optics, DOF, lighting,
environment editing, character import and animation, Root Motion, V10 keyframe easing,
V11 Cinematic Sequencer, and Auto/Desktop/Tablet layouts.

NEW IN V12
1. Export complete stage as binary GLB (.glb) using Three.js GLTFExporter.
2. Optional inclusion of animation clips embedded in imported rigged GLB/GLTF characters.
3. Export project manifest JSON containing editable primitive scene data, camera settings,
   and the V11 camera sequence.
4. Existing Scene JSON and Camera Sequence JSON exports remain available.

HOW TO EXPORT
- Import your character and add/edit scene objects.
- Configure lighting and frame the scene.
- In Environment Studio, find Export studio · deliverables.
- Choose whether to include embedded character animations.
- Click Export complete scene (.glb).
- Click Export project manifest (.json) to save editable scene metadata and camera sequence.
- The V11 Cinematic Sequencer can also save its camera sequence JSON independently.

INSTALL
1. Extract this ZIP on your computer.
2. Open:
   https://github.com/ctaccc2727/MILO-MIMI-virtual-cinematographer
3. Add file -> Upload files.
4. Upload the extracted index.html and README.txt from this V12 folder to the repository root.
   Do NOT upload the ZIP itself.
5. Commit changes, wait for GitHub Pages, then hard refresh with Ctrl+F5.

IMPORTANT LIMITATIONS
- GLB export contains the stage contents (models and scene objects) but does not bake the
  live camera sequencer into a rendered movie.
- Camera sequence and editable project manifest are separate JSON deliverables.
- The manifest references scene object data; the GLB is the companion file containing geometry.
- Exported animation support depends on the imported model's embedded animation clips and
  GLTFExporter compatibility. Custom V10/V9 pose-timeline animation is not yet baked into GLB.
- This release is statically syntax-checked and ZIP-integrity checked; it has not been physically
  tested on the user's browser/tablet in this session.
