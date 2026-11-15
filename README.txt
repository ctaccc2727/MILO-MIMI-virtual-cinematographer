VIRTUAL CINEMATOGRAPHER — V10 ANIMATION EDITOR

V10 extends V9 and retains all previous modules:
camera/optics/DOF, lighting, environment, character import, skeleton inspector,
custom pose timeline, Root Motion, and Auto/Desktop/Tablet layout modes.

NEW IN V10
- Edit selected keyframe time numerically.
- Choose interpolation into a keyframe: Linear, Ease In, Ease Out, Ease In/Out, Hold/Step.
- Sort keyframes by time.
- Keyframe easing and Root Motion data are saved in animation JSON.
- V8/V9 animation JSON remains loadable; missing easing defaults to Ease In/Out.

INSTALL
1. Extract this ZIP on your computer.
2. Open the GitHub repository:
   https://github.com/ctaccc2727/MILO-MIMI-virtual-cinematographer
3. Add file -> Upload files.
4. Upload the extracted index.html and README.txt from this V10 folder to the repository root.
   Do NOT upload the ZIP itself.
5. Commit changes, wait for GitHub Pages, then hard-refresh with Ctrl+F5.

NOTES
- Easing is applied to the transition INTO each selected destination keyframe.
- Hold/Step keeps the previous pose/root transform until the destination keyframe.
- This editor does not yet provide a visual graph-curve drawing surface.
- This release is statically syntax-checked; it has not been physically tested on your browser/tablet.
