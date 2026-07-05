# Components

Components are the smallest reusable UI pieces in the Elyx design system. Think 
of them as atoms.They sit above shared tokens and assets, and below blocks and
screens:

```
tokens / icons / images
  -> components
    -> blocks
      -> screens
```

A component should be focused enough to reuse in more than one place without
bringing along screen-specific layout or product context. Use this folder for
base controls, small grouped controls, and reusable interface primitives such as
buttons, inputs, toggles, rows, swatches, dividers, toolbar controls, and
similar pieces.

## Best Practices

- Keep one primary reusable component per file when practical.
- Import shared values from `tokens.elyx` instead of hard-coding repeated
  colors, spacing, typography, or radii.
- Expose intended reuse with `pub`; keep helper layers private unless another
  file needs to import them.
- Name files and public symbols for the component's role, not for the first
  screen that used it.
- Keep component layout local and minimal. A component can define its own shape,
  padding, states, and internal alignment, but should avoid positioning itself
  for a specific screen.
- Use variants for meaningful component states such as hover, pressed, selected,
  disabled, or reusable colorways when those states are part of the component
  contract.
- Prefer composition over duplication. If the same control appears in multiple
  blocks or screens, extract it here and import it.
- Avoid showcase or demo layouts in component files unless the file is
  intentionally documenting variants.

Larger reusable interface sections belong in `design/blocks/`. Complete
surfaces or top-level states belong in `design/screens/`.
