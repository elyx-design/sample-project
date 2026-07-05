# Blocks

Blocks are reusable UI sections composed from components. They sit between
small controls (comoponents) and complete screens:

```
tokens / icons / images
  -> components
    -> blocks
      -> screens
```

A block should be larger than a single control, but smaller than a complete
screen. Use blocks for recognizable interface sections such as panels, menus,
toasts, alerts, etc that would contain component(s).

## Best Practices

- Compose blocks from `design/components/` and shared values from
  `tokens.elyx` wherever possible.
- Keep blocks portable within their product area. They may know they are an
  inspector section, sidebar group, or toolbar composition, but should avoid
  assuming the full window around them unless that is the point of the block.
- Use one file for one primary block or closely related block family when
  practical.
- Expose only the block entry points that screens or other blocks should import
  with `pub`.
- Keep nested helper layers private unless they are intentionally part of the
  import contract.
- Prefer variants for alternate block states over duplicating near-identical
  files.
- Extract repeated block-sized UI out of screens into this folder.
- If a block grows into a complete surface or top-level state, move that work to
  `design/screens/`.

Single primitive controls belong in `design/components/`.
