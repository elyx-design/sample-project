# Controls

Controls are the smallest reusable UI elements in the Elyx design system. Buttons, inputs, avatars, tags, dividers, and similar elements belong here.

## Guidelines

- Keep one primary reusable control per file when practical.
- Import shared values from `tokens/` instead of repeating them.
- Export the variants other files should reuse.
- Name controls for their role, not the first screen that used them.
- Keep layout local to the control.
- Use variants for states such as hover, pressed, selected, and disabled.
- Keep prototype navigation out of controls.
- Do not import from `design/blocks/`, `design/screens/`, or `design/flows/`.

Compositions of several controls belong in `design/blocks/`.
