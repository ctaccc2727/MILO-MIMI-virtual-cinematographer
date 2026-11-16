VIRTUAL CINEMATOGRAPHER — V16 MOTION BINDING FIX

Based on V15. All existing modules and features are retained.

V16 change:
- Motion Studio animation tracks now bind to the target Three.js node by UUID rather than display name.
- This avoids ambiguous/empty/duplicate node-name binding in imported GLB hierarchies.
- GLB export status reports the generated Motion clip names and count.

Test:
1. Replace index.html and README.txt in the GitHub repository root.
2. Commit, wait for GitHub Pages, then Ctrl+F5.
3. Import StockClerk and select it in Environment Studio → Scene objects.
4. Create at least two Motion Studio keyframes and verify playback.
5. Export complete scene (.glb) with Include animations checked.
6. Read the export status: it should report e.g. 8 animation clips (1 Motion: Motion_StockClerk).
7. Open the new GLB in glTF Viewer → Animation and check for the extra Motion clip.

Notes:
- The UUID binding fix addresses track-to-node resolution; it is a targeted correction, not a guarantee until the user's new GLB is inspected.
- Do not change the trajectory or coordinate signs yet. First verify that the extra Motion clip is present. Then compare direction.
- Static JavaScript syntax and ZIP integrity are checked; browser behavior still needs user verification.
- Keep .nojekyll; do not upload this ZIP itself.
