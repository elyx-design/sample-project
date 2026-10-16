# Project context

This is the Elyx sample project. `.elyx` files contain the designs, and
`elyx.json` contains project settings. `readme.md` introduces the project.

## Structure

- `design/controls/` holds the smallest reusable elements, such as buttons, text
  fields, tags, and avatars.
- `design/blocks/` combines controls into reusable sections, such as cards,
  forms, menus, and navigation areas.
- `design/screens/` holds complete views and standalone states.
- `design/flows/` collects screens on one canvas and connects them into
  journeys.
- `tokens/` holds shared colors, typography, spacing, radii, and strings, with
  dark theme and French locale overrides.
- `images/` and `icons/` hold the project's assets. New assets are written to
  `images/`.
- `index.elyx` is the project's welcome canvas.

Each folder has a `README.md` with its own guidelines. Read it before changing
files in that folder.

## Dependency direction

```text
tokens / icons / images
  -> design/controls
    -> design/blocks
      -> design/screens
        -> design/flows
```

Imports may stay within a layer or point to a lower layer. They must not point
upward. For example, a control must not import a block, and a block must not
import a screen.

## Working in this project

- Follow the patterns in existing `.elyx` files.
- Reference tokens instead of repeating colors, sizes, and strings.
- Keep this file current as the project evolves.
