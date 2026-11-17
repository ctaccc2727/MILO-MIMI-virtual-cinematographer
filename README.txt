VIRTUAL CINEMATOGRAPHER V19 — RENDER QUALITY

Based on V18. All previous studios, project ZIP save/load, camera sequencing, and WebM recording remain included.

V19 adds:
- Render quality profiles: Compact, Balanced, High, Custom.
- Selectable target video bitrate: 4, 8, 12, or 16 Mbps.
- Compact: 720p / 24 fps / 4 Mbps.
- Balanced: 720p / 30 fps / 8 Mbps.
- High: 1080p / 30 fps / 12 Mbps.
- Export preview summary before recording.
- Render settings are remembered in the browser on that device.

Important:
- Bitrate is a target requested from MediaRecorder; actual encoding may vary by browser.
- This is real-time browser capture, not offline/path-traced rendering.
- WebM only; no audio, MP4/H.264, 4K, offline rendering, or shadow-map quality controls.
- High resolution/bitrate may be demanding. Use Compact or Balanced if recording stutters.
- Keep the browser tab active while recording.

Install:
1. Extract this ZIP.
2. Upload index.html and README.txt to the root of your GitHub Pages repository, replacing previous files.
3. Commit changes and wait for GitHub Pages.
4. Refresh with Ctrl+F5.

Do not upload check.mjs. Keep .nojekyll in the repository.
External CDN access is required for Three.js modules.

Validation:
ZIP integrity and JavaScript syntax are checked. This build has not been browser-tested on your device.
