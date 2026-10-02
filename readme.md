# Demo Project

Welcome to the Elyx demo project.

This project demonstrates how to organize and build `.elyx` files. An Elyx project consists of many components so we've organied our UI files in the `design/` in four folders:

```text
design/
  controls/
  blocks/
  screens/
  flows/
```

## Controls

Here we've stored components that are the smallest reusable UI elements. Buttons, text fields, tags, avatars, and similar elements. We've called them "Controls" but that is just the name of the folder: `design/controls/`.

## Blocks

Similarly, larger components are stored here. We've called the fodler "Blocks". They combine controls into reusable interface sections such as cards, menus, forms, and navigation areas. They belong in `design/blocks/`.

## Screens

Elyx encourages you to even create components out of entire screens; our overrides system is powerful enough to make that work like a charm.
Screens are complete views or standalone states. Sign in, pricing, and editor views belong in `design/screens/`.

## Flows

To help you visualise flows in your product it can be helpful to collect multiple screens into a single file and draw connections between them.
We like to organise these elyx files into the `design/flows/` folder. Useful when a prototype needs multi-screen paths or flow-specific annotations.

Tokens and assets remain at the project root. `tokens/` contains shared colors, typography, spacing, strings, and radii. Images and icons live in their matching asset folders.
