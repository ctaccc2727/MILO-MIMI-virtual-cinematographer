VIRTUAL CINEMATOGRAPHER V30 — AI SCENE BUILDER

Install: replace index.html and README.txt in the GitHub Pages repository root. Keep .nojekyll.

New module: AI Scene Builder. Paste a director prompt containing headings like:
SHOT 1 · 0:00–0:04 · TITLE
SHOT 2 · 0:04–0:07 · TITLE

Click Build scene & camera sequence. The module parses shot headings, durations and basic camera intent, creates camera entries, and updates the existing Cinematic Sequencer. Export scene plan downloads a JSON breakdown with the prompt, shot descriptions, reference filenames and environment bounds.

Important capability boundary: this is a local deterministic prompt parser and camera-blocking assistant. It does not call an external generative AI model and does not create rigged 3D character assets from still images. Character reference images must still be supplied to the video generator; rigged character models require separate 3D assets.

Existing V29 functions are retained. Imported GLB models remain source assets and should be re-imported after loading a project if not embedded in the project archive.
