# Design

UI definitions follow this dependency direction:

```text
tokens / icons / images
  -> design/controls
    -> design/blocks
      -> design/screens
        -> design/flows
```

Imports may stay within a layer or point to a lower layer. They must not point upward. For example, a control must not import a block, and a block must not import a screen.

- `controls/` contains focused reusable elements.
- `blocks/` contains reusable compositions.
- `screens/` contains complete views and standalone states.
- `flows/` connects screens into journeys.
