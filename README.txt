VIRTUAL CINEMATOGRAPHER V18 — RENDER STUDIO

Based on V17. All previous studios and project save/load features are retained.

V18 adds:
- Record view: records the current 3D viewport.
- Render sequence: records the Cinematic Sequencer automatically from start to finish.
- Output resolution: current viewport, 1280×720 HD, or 1920×1080 Full HD.
- Frame rate: 24, 30, or 60 fps.
- WebM export using the browser MediaRecorder API.
- Elapsed recording timer and status.
- Automatic restoration of the original viewport dimensions after recording.

Important limitations:
- This is real-time browser capture, not an offline/path-traced renderer.
- Video is exported as WebM. No audio is recorded.
- 4K, MP4/H.264 encoding, offline rendering, and render-quality/shadow presets are not included.
- 1080p/60 fps may be too demanding on some devices; use 720p/24 or 30 fps if recording stutters.
- Keep the browser tab active during recording. Performance depends on browser, GPU, scene complexity, and device.
- If the browser does not support MediaRecorder or canvas capture, recording will be unavailable.

Install:
1. Extract this ZIP.
2. Upload index.html and README.txt to the root of your GitHub Pages repository, replacing the previous files.
3. Commit changes and wait for GitHub Pages to publish.
4. Refresh with Ctrl+F5.

Do not upload check.mjs. Keep .nojekyll in the repository.
External CDN access is required for Three.js modules.

Validation:
ZIP integrity and JavaScript syntax are checked. This build has not been browser-tested on your device.
