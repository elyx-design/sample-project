# Blocks

Blocks are reusable UI sections composed from controls or other blocks. Cards, forms, menus, toolbars, and navigation areas belong here.

## Guidelines

- Compose blocks from `design/controls/` and shared values from `tokens/`.
- A block may import another block when that composition remains reusable.
- Keep blocks portable within their product area.
- Export only the entry points screens and other blocks need.
- Prefer variants over near-identical files.
- Keep screen-level placement and journeys out of blocks.
- Do not import from `design/screens/` or `design/flows/`.

Complete views belong in `design/screens/`. Single controls belong in `design/controls/`.
