# Getting Started with Quickpolicy Design System

Welcome to the Quickpolicy Design System! This guide will help you understand and use the components in this repository.

## What is This?

This is a design system containing UI components converted from Figma designs into clean, production-ready HTML and CSS. Each component is:
- **Self-contained**: Works independently without dependencies on frameworks
- **Customizable**: Uses CSS variables (design tokens) for easy theming
- **Well-documented**: Includes usage examples and guidelines
- **Accessible**: Built with web accessibility standards in mind

## Quick Start Guide

### 1. Explore the Components

Navigate to the `components/` folder to see available components organized by category:
- `buttons/` - Button components
- `cards/` - Card components
- `forms/` - Form elements
- `navigation/` - Navigation components

### 2. Preview a Component

Each component has an `index.html` file that you can open directly in your browser:

```bash
# Example: View the Get Started button
open components/buttons/get-started/index.html
```

### 3. Use in Your Project

**Method A: Copy Files**
1. Copy the component's CSS file to your project
2. Copy `styles/variables.css` for design tokens
3. Link them in your HTML:
   ```html
   <link rel="stylesheet" href="variables.css">
   <link rel="stylesheet" href="get-started.css">
   ```
4. Use the component's HTML structure

**Method B: Copy Code**
1. Open the component's HTML file
2. Copy the HTML structure you need
3. Copy the CSS from the `.css` file
4. Paste into your project

## Understanding Design Tokens

Design tokens are the foundational values of the design system, defined in `styles/variables.css`.

### Colors
```css
--primary-purple: rgb(147, 102, 221);
--border-light-purple: #dccaf9;
--text-white: #ffffff;
```

### Spacing
```css
--spacing-sm: 8px;
--spacing-md: 12px;
--spacing-lg: 16px;
--spacing-xl: 20px;
```

### Typography
```css
--font-size-base: 16px;
--font-size-xl: 20px;
--font-weight-medium: 500;
```

### Using Tokens
```css
.my-element {
  color: var(--primary-purple);
  padding: var(--spacing-md);
  font-size: var(--font-size-xl);
}
```

## Component Structure

Each component follows this structure:

```
component-name/
├── index.html           # Standalone demo page
├── component-name.css   # Component styles
└── README.md           # Documentation and usage guide
```

## Customizing Components

### Option 1: Override CSS Variables
```css
:root {
  --primary-purple: rgb(100, 50, 200); /* Your brand color */
}
```

### Option 2: Add Custom Classes
```css
.btn-get-started.my-custom-button {
  padding: 20px 40px;
  font-size: 24px;
}
```

### Option 3: Modify the CSS File
Create a copy of the component and modify it to fit your needs.

## Best Practices

### 1. Use Semantic HTML
Components use semantic HTML elements (`<button>`, `<nav>`, etc.) for better accessibility.

### 2. Maintain Design Tokens
When customizing, try to use existing design tokens instead of hardcoding values.

### 3. Test Across Browsers
Always test components in your target browsers before deploying.

### 4. Consider Accessibility
- Ensure keyboard navigation works
- Test with screen readers
- Maintain sufficient color contrast
- Add ARIA labels where needed

### 5. Keep Components Modular
Don't add unnecessary dependencies or coupling between components.

## Common Tasks

### Adding a New Component
See the [Contributing section](../README.md#contributing) in the main README.

### Changing Colors
Edit `styles/variables.css` to update colors across all components:
```css
:root {
  --primary-purple: #your-color;
}
```

### Adjusting Spacing
Modify spacing tokens in `variables.css`:
```css
:root {
  --spacing-md: 14px; /* Changed from 12px */
}
```

### Creating Variations
Create new CSS classes that extend existing components:
```css
.btn-get-started.btn-secondary {
  background: var(--secondary-color);
  border-color: var(--secondary-border);
}
```

## Folder Organization

```
├── components/          # All UI components
│   └── [category]/     # Category folders (buttons, cards, etc.)
│       └── [component]/ # Individual component folder
├── pages/              # Full page examples
├── styles/             # Global styles and tokens
│   └── variables.css   # Design tokens
└── docs/               # Documentation
    └── GETTING_STARTED.md # This file
```

## Need Help?

- Check component-specific READMEs in each component folder
- Read the main [README.md](../README.md) for project overview
- Open an issue on GitHub for bugs or questions
- Contact the design system team

## Next Steps

1. **Explore**: Browse through the components folder
2. **Experiment**: Open component demos in your browser
3. **Implement**: Copy components into your project
4. **Customize**: Adjust design tokens to match your brand
5. **Contribute**: Add new components following our guidelines

---

**Happy coding!** 🚀

For more information, see the [main README](../README.md).
