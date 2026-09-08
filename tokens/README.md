# Tokens

Tokens are shared values referenced throughout the Elyx design system. They
provide a single source of truth for colors, strings, spacing, typography, and
corner radii, and sit beneath the design hierarchy:

```
tokens / icons / images
  -> design/controls
    -> design/blocks
      -> design/screens
        -> design/flows
```

Use `tokens/` for values that should remain consistent across multiple files.
Theme and locale files can extend the default token sets with contextual values,
as demonstrated by `colors.dark.elyx` and `strings.fr.elyx`.

## Best practices

- Group related token families into focused files such as `colors.elyx`,
  `spacing.elyx`, `typography.elyx`, `radius.elyx`, and `strings.elyx`.
- Within `colors.elyx`, keep fixed values in `primitives` and `palette`, and group
  contextual values by role in `theme`, `status`, `controls`, and `surfaces`.
- Use `base` and `contrast` names for theme-dependent neutral colors, and omit
  prefixes already supplied by a group name, such as `status.visible` and
  `controls.foreground`.
- Export token sets that other files need to import.
- Reference tokens instead of hard-coding values that appear in multiple places.
- Use clear names that describe a token's purpose or value consistently.
- Keep the same token structure in theme and locale overrides so references remain
  stable across contexts.
- Define default values in the base token file and only override values that need
  to change for a theme or locale.
- Keep units and naming patterns consistent within each token family.
- Store reusable values here, but keep component structure and screen-specific
  layout in their appropriate folders.

Reusable UI elements belong in `design/controls/`, larger interface sections
belong in `design/blocks/`, and complete views belong in `design/screens/`.
