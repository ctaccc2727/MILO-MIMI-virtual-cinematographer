VIRTUAL CINEMATOGRAPHER V22 — RENDER INITIALIZATION FIX

Based on V21. Retains all previous studios and features.

V22 fix:
- Fixed a JavaScript temporal-dead-zone error in Render Quality initialization.
- The GPU anisotropy capability is now read inside renderApplyQuality(), after module initialization reaches the function call.
- This prevents the error "Cannot access 'renderMaxAnisotropy' before initialization" from aborting 3D scene startup.

Install:
1. Extract this ZIP.
2. Replace index.html and README.txt in the root of your GitHub Pages repository.
3. Commit changes and wait for deployment.
4. Refresh with Ctrl+F5.

Do not upload check.mjs. Keep .nojekyll.
External CDN access is required.

Validation:
ZIP integrity and JavaScript syntax checked. This build has not been browser-tested on your device.
