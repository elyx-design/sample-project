# Design

We've organized our Elyx design files in folders, divided roughly by size;

- "controls" for small elements like buttons
- "blocks" for larger elements that combine controls; think panels, menus, cards and forms
- "screens" for the largest components that capture entire screens; login screens, account screens etc.

Think of Elyx as a knowledge base that captures the state of a project. The knowledge of what a project is goes way beyond what you may traditionally call a "design system" (which was always a glorified bucket of styles and buttons). We encourage you to create components for the larger states as well. This in turn then feeds in to teaching agents about your project.


# Agent Instructions

Because Elyx is just plain text files on your computer, an agent navigates Elyx files just as it would html files and  it will read these markdown files too. So you can put agent-specific instructions in here.

For example:

UI definitions follow this dependency direction:

```text
tokens / icons / images
  -> design/controls
    -> design/blocks
      -> design/screens
        -> design/flows
```

Imports may stay within a layer or point to a lower layer. They must not point upward. For example, a control must not import a block, and a block must not import a screen.