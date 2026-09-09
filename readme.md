# Demo Project

Welcome to the Elyx demo project.

This project demonstrates how to organize and build `.elyx` files. UI files live under `design/` in four layers:

```text
design/
  controls/
  blocks/
  screens/
  flows/
```

## Controls

Controls are the smallest reusable UI elements. Buttons, text fields, tags, avatars, and similar elements belong in `design/controls/`.

## Blocks

Blocks combine controls into reusable interface sections such as cards, menus, forms, and navigation areas. They belong in `design/blocks/`.

## Screens

Screens are complete views or standalone states. Sign in, pricing, and editor views belong in `design/screens/`.

## Flows

Flows connect screens into journeys. Use `design/flows/` when a prototype needs multi-screen paths or flow-specific annotations.

Tokens and assets remain at the project root. `tokens/` contains shared colors, typography, spacing, strings, and radii. Images and icons live in their matching asset folders.
