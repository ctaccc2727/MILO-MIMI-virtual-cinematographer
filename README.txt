VIRTUAL CINEMATOGRAPHER — V11 CINEMATIC SEQUENCER

V11 extends V10 and retains all previous modules: camera controls and optics, DOF,
lighting, environment editing, character import and animation, Root Motion, keyframe
easing editor, and Auto/Desktop/Tablet layouts.

NEW IN V11 — CINEMATIC SEQUENCER
- Capture the current viewport camera as a shot.
- Store camera position, orientation, focal length, sensor, aperture, focus and DOF settings.
- Build an ordered multi-shot sequence.
- Set each shot duration.
- Choose the transition into the next shot: Smooth camera move, Linear camera move, or Hard cut.
- Replace or delete selected shots.
- Play and stop the sequence.
- Scrub the sequence timeline.
- Save and load sequence JSON.

HOW TO USE
1. Frame the desired angle in the 3D viewport using mouse/WASD and camera optics.
2. In Cinematic Sequencer, choose shot duration and transition.
3. Click Capture current shot.
4. Frame another angle and capture the next shot.
5. Repeat for additional shots.
6. Click Play sequence. Use the timeline slider to scrub.
7. Save sequence JSON to reuse the camera edit later.

INSTALL
1. Extract this ZIP on your computer.
2. Open:
   https://github.com/ctaccc2727/MILO-MIMI-virtual-cinematographer
3. Add file -> Upload files.
4. Upload extracted index.html and README.txt from this V11 folder into repository root.
   Do NOT upload the ZIP itself.
5. Commit changes, wait for GitHub Pages, then hard refresh with Ctrl+F5.

NOTES / LIMITATIONS
- This is a camera sequencer: it stores and plays camera shots, not a rendered video export.
- Smooth and Linear transitions interpolate camera position, orientation and focal length.
- Hard cut holds the current shot and switches at its duration boundary.
- Audio tracks, clip trimming, rendered video export, and multi-track editing are not included yet.
- Statically syntax-checked and ZIP integrity checked; not physically tested on the user's browser/tablet in this session.
