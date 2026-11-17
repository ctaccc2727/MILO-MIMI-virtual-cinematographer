VIRTUAL CINEMATOGRAPHER V17 — PROJECT RESTORE FIX

Based on V16. Retains the previous studios and features.

V17 fixes:
- Complete Project ZIP now preserves Custom Timeline keyframes even if the character selector is not actively focused, provided custom keyframes exist.
- On project load, Motion Studio automatically selects the saved Motion target object.
- Motion duration/timeline range is restored from the saved target's keyframe times.
- Load status reports the restored Motion and Custom keyframe counts.
- Character matching handles empty saved character names by falling back to the available rigged character.

Install:
1. Extract this ZIP.
2. Upload index.html and README.txt to the root of your GitHub Pages repository, replacing the previous files.
3. Commit changes and wait for GitHub Pages to publish.
4. Refresh the site with Ctrl+F5.

Do not upload check.mjs. Keep .nojekyll in the repository.
External CDN access is required for Three.js and JSZip modules.

Validation note:
This package was checked for JavaScript syntax and ZIP integrity. It has not been browser-tested on your device.
