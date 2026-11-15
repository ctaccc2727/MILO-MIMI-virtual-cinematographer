VIRTUAL CINEMATOGRAPHER — V9 ROOT MOTION STUDIO

V9 extends V8 and retains its camera, optics, DOF, lighting, environment, character import,
skeleton inspector, custom pose timeline, and Auto/Desktop/Tablet layout modes.

NEW IN V9
- Move the selected character root in X, Y, Z.
- Set character heading (Yaw) in degrees.
- Move by directional buttons relative to the character's current heading.
- Reset root transform to the character's imported starting position.
- Root position and heading are captured with each custom animation keyframe.
- Root position and heading interpolate between custom keyframes.
- V9 animation JSON stores root transforms and remains able to load older V8 animation JSON
  (older files simply have no root-motion data).

INSTALL
1. Extract this ZIP on your computer.
2. Open your GitHub repository:
   https://github.com/ctaccc2727/MILO-MIMI-virtual-cinematographer
3. Choose Add file -> Upload files.
4. Upload the extracted index.html and README.txt from this V9 folder to the repository root.
   Do NOT upload the ZIP itself.
5. Commit changes.
6. Wait for GitHub Pages to publish, then open:
   https://ctaccc2727.github.io/MILO-MIMI-virtual-cinematographer/
7. Hard refresh with Ctrl+F5.

IMPORTANT
- Use a rigged character for bone pose animation. Root movement also works for imported 3D models.
- Root movement is scene-level positioning; it does not automatically create foot-contact or walk-cycle animation.
- To animate travel, create custom keyframes at different times and use Play Custom.
- This release is statically syntax-checked; it has not been physically tested on your tablet/browser in this session.
