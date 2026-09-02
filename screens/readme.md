# Screens

Screens are complete UI surfaces or standalone screen-level states assembled
from blocks, components, tokens, and assets. They sit above reusable sections
(blocks).

```
tokens / icons / images
  -> components
    -> blocks
      -> screens
```

Use `screens/` for complete views or standalone states that represent what a
user sees at a given moment, such as Sign in, Dashboard, Settings, or Account.

## Best practices

- Prefer one top-level screen or screen state per file.
- Compose screens from `blocks/` and `components/` instead of
  duplicating reusable UI directly in the screen file.
- Import shared tokens, icons, images, and fonts rather than embedding copied
  values or artwork.
- Treat screen files as composition layers. They can own page-level placement,
  app-window structure, and state-specific overrides, but reusable controls and
  sections should usually live lower in the hierarchy.
- Use clear names that describe the visible state, such as a window, panel, or
  onboarding step.
- Keep public exports focused on the screen states that other files, especially
  flows, need to import.
- Use overrides to adapt imported blocks and components for the screen state
  instead of forking the source component for one-off differences.

Lower-level reusable pieces belong in `components/` and `blocks/`. Shared visual
values belong in `tokens/`.
