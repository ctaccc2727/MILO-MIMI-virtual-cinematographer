VIRTUAL CINEMATOGRAPHER — V14 MOTION STUDIO

V14 is based on V13 and retains its features:
- Camera controls, optics and depth of field
- Lighting Studio and Environment Studio
- GLB/GLTF import, character animation and skeleton inspector
- Root Motion, custom pose timeline and keyframe easing
- Cinematic Sequencer
- Complete project ZIP save/load
- Auto / Desktop / Tablet layouts

NEW IN V14 — MOTION STUDIO
- Select a scene object or character root in Environment Studio → Scene objects.
- Set Motion duration and move the timeline to a time.
- Position/rotate the target using the existing object transform controls or root controls.
- Click Capture transform to add a keyframe.
- Move to another time, transform the target and capture again.
- Play motion to preview interpolated position and quaternion rotation.
- Update at time replaces/creates a key at the current time.
- Delete selected key removes the key nearest the current playhead.
- Clear target track removes the selected target's motion track.
- Motion tracks are included in complete project ZIP archives.
- GLB export adds generated position/quaternion animation clips for tracks with at least two keys.

IMPORTANT LIMITATIONS
- Motion Studio animates the selected object's root transform. It does not create footstep animation or edit internal skeleton bones; use the existing custom pose timeline for bone posing.
- Root-motion clips and imported skeletal clips are exported as GLB animation clips. They are separate clips, not automatically blended together.
- If multiple scene objects share the same object name, rename them uniquely before creating motion tracks.
- Camera synchronization remains handled by the existing Cinematic Sequencer; V14 does not yet bake camera animation into the scene GLB.
- Complete project ZIP uses JSZip and Three.js modules from jsDelivr; internet access is required.
- This build is statically syntax-checked and ZIP-checked. Actual browser/device behavior must be verified in the user's browser.

INSTALL
1. Extract this ZIP.
2. GitHub repository:
   https://github.com/ctaccc2727/MILO-MIMI-virtual-cinematographer
3. Add file → Upload files.
4. Upload index.html and README.txt from this V14 folder to repository root, replacing the old files.
5. Commit changes, wait for GitHub Pages, then Ctrl+F5.
6. Do not upload this ZIP itself. Keep .nojekyll.
