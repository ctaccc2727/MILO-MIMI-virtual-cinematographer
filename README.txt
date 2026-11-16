VIRTUAL CINEMATOGRAPHER — V15 MOTION EXPORT FIX

V15 is based on V14 and retains all previous features.

FIX
The standalone Export complete scene (.glb) action now includes:
- Imported character animation clips
- Generated Motion Studio transform clips (Motion_<object name>)
when the existing Include animations checkbox is enabled.

The V14 bug:
- Complete project ZIP export collected Motion Studio tracks.
- Standalone GLB export collected only imported animation clips.
- Therefore Motion Studio movement did not appear as an additional clip in glTF Viewer.

TEST
1. Install V15 by replacing index.html and README.txt in the GitHub repository root.
2. Hard refresh with Ctrl+F5.
3. Import the character and create at least two Motion Studio keyframes.
4. In Export Studio, ensure Include animations is checked.
5. Click Export complete scene (.glb).
6. Open the new GLB in glTF Viewer → Animation.
7. Look for Motion_<character/object name> in addition to the imported clips.
8. The export status should report the total clip count and number of Motion clips.

IMPORTANT
- This fixes the missing Motion clip collection in the standalone GLB export.
- It does not yet claim to fix the apparent forward/backward Z-direction difference. First verify that the Motion clip is present and plays. Then compare its trajectory; a separate coordinate/root-parent correction may be needed.
- Static syntax and ZIP checks passed; browser testing remains to be performed by the user.
- Keep .nojekyll. Do not upload this ZIP itself.
