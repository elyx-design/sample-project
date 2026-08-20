# Scaffold

This document contains best practices on how to set up .elyx files within your project

As you can see in the project list on the left, files are organized into groups, with 
the most important ones being components, blocks, and screens. The three main building 
blocks for organizing your components.

## Components
Components are the smallest reusable UI pieces in the Elyx design system. Think of them 
like atoms. These would be UI elements such as button, text fields, badges etc.

## Blocks
If components are atoms, then blocks are like molecules. Blocks are used interface 
sections such as panels, menus, toasts, alerts, etc that would contain components.

## Screens
Screens would be things like app windows, panels, and standalone states that represent 
what a user would see at one moment. Examples would be things like Log In, Dashboard, 
Settings, Account, etc.

Also in the project are folders for other asset types, such as images and icons. If you 
were to add fonts, then create a new /fonts folder.

Finally, is the existence of a tokens/ folder. Each file there groups a related family of
tokens - colors, typography, spacing, radius - referenced throughout the entire project.