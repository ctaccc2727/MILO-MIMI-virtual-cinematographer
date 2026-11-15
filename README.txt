VIRTUAL CINEMATOGRAPHER V4.1 FIX

This is a corrective continuation of V4.

Important fix:
- The base Three.js scene now starts and renders independently of the optional Depth of Field post-processing modules.
- EffectComposer, RenderPass and BokehPass are loaded dynamically after the base scene is ready.
- If a post-processing module fails to load or crashes during rendering, the app falls back to direct renderer.render(scene, camera).
- The user can still use the scene, camera controls and optics without DOF.
- DOF controls are disabled when the effect cannot be initialized.

Retained:
- V3 optics: Full Frame, Super 35, ALEXA 35, focal length, aperture and focus distance.
- V4 DOF controls and Rack Focus demo when post-processing is available.
- Free, Cinematic and Orbit camera modes.
- Desktop keyboard/mouse and on-screen controls.
- Tablet touch joysticks.
- Camera preset JSON save/load.

Checks:
- JavaScript syntax checked with Node.
- ZIP integrity checked.
- Duplicate HTML IDs checked.

Internet access is required for Three.js and optional post-processing modules.

V4.2 FIX:
- Added a browser import map for the bare module specifier `three`.
- Three.js post-processing example modules (EffectComposer, RenderPass, BokehPass) import `three` by package name. Without an import map, browsers cannot resolve that package name from CDN-loaded ES modules, so DOF initialization failed and the toggle remained disabled/OFF.
- The DOF button now displays UNAVAILABLE if initialization genuinely fails, rather than misleadingly displaying OFF.

V4.3 DOF FIX:
- Corrected the BokehPass aperture scale. The previous value (0.00002) was orders of magnitude below the Three.js BokehPass example scale (0.025), making the blur effectively imperceptible.
- Default blur strength raised to 18/30 for a visible test while retaining a capped maxblur of 0.018.
- Rack Focus Demo now sweeps through 6.5, 8.5 and 11.5 scene units, closer to the depths of the sample scene from the default camera.
- Focus is the distance along the camera view in scene units, as defined by Three.js BokehPass.

GitHub Pages deployment package: upload these extracted files to the repository root.
