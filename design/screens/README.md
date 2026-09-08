# Screens

Screens are complete UI views or standalone states assembled from blocks, controls, tokens, and assets.

## Guidelines

- Prefer one top-level screen or screen state per file.
- Compose screens from `design/blocks/` and `design/controls/`.
- Keep reusable sections out of screen files.
- Let screens own page-level placement and state-specific overrides.
- Keep exports focused on states that other screens or flows need.
- Screens may link to other screens for prototype navigation.
- Do not import from `design/flows/`.

Multi-screen journey canvases and flow-specific annotations belong in `design/flows/`.
