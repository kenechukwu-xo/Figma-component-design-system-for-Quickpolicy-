# Figma Component Design System for Quickpolicy

A professional design system built from Figma designs, converted to clean HTML and CSS components for easy implementation.

## 🌐 Live Demo

**[View Component Gallery →](https://kenechukwu-xo.github.io/Figma-component-design-system-for-Quickpolicy-/)**

Browse all components with live previews, search functionality, and interactive examples.

## 📋 Overview

This repository contains production-ready UI components converted from Figma designs. Each component is built with:
- Semantic HTML5
- Clean, maintainable CSS
- Design tokens for consistency
- Standalone examples for easy testing
- Documentation for quick implementation

## 🚀 Quick Start

1. **Clone the repository**
   ```bash
   git clone https://github.com/kenechukwu-xo/Figma-component-design-system-for-Quickpolicy-.git
   cd Figma-component-design-system-for-Quickpolicy-
   ```

2. **View components**
   - Open any HTML file in the `components` folder directly in your browser
   - Each component is self-contained and ready to use

3. **Use in your project**
   - Copy the component's HTML and CSS files to your project
   - Import `styles/variables.css` for design tokens
   - Customize as needed using the CSS variables

## 📁 Project Structure

```
Figma-component-design-system-for-Quickpolicy-/
├── components/           # All UI components
│   ├── buttons/         # Button components
│   ├── cards/           # Card components
│   ├── forms/           # Form elements (inputs, selects, etc.)
│   └── navigation/      # Navigation components (navbars, menus, etc.)
├── pages/               # Full page examples
├── styles/              # Global styles and design tokens
│   └── variables.css    # CSS custom properties (colors, spacing, etc.)
├── docs/                # Documentation and guides
└── README.md            # This file
```

## 🎨 Design Tokens

Design tokens are defined in `styles/variables.css` and include:
- **Colors**: Primary palette, text colors, borders
- **Spacing**: Consistent spacing scale (xs to 3xl)
- **Typography**: Font families, sizes, weights
- **Shadows**: Elevation system for depth
- **Border Radius**: Consistent corner rounding
- **Transitions**: Standard animation durations

### Using Design Tokens

```html
<!-- Include variables in your HTML -->
<link rel="stylesheet" href="../styles/variables.css">
```

```css
/* Use variables in your CSS */
.my-button {
  background-color: var(--primary-purple);
  padding: var(--spacing-md) var(--spacing-xl);
  border-radius: var(--radius-xl);
  font-size: var(--font-size-xl);
}
```

## 🔧 How to Use Components

### Method 1: Direct Usage
1. Navigate to the component folder (e.g., `components/buttons/`)
2. Open the HTML file in a browser to preview
3. Copy the HTML and CSS to your project
4. Adjust as needed

### Method 2: Integration
1. Copy the component's CSS file to your project's stylesheet
2. Import `variables.css` for design tokens
3. Use the component's HTML structure in your pages
4. Customize using CSS variables or override styles

## 🤝 Contributing

We welcome contributions from team members! Here's how to add new components:

### Adding a New Component

1. **Create the component files**
   ```
   components/[category]/[component-name]/
   ├── index.html          # Standalone demo
   ├── [component-name].css # Component styles
   └── README.md           # Component documentation
   ```

2. **Follow the structure**
   - Use semantic HTML5
   - Reference design tokens from `variables.css`
   - Keep components modular and reusable
   - Include a standalone demo in `index.html`

3. **Document your component**
   - Add a README.md explaining usage
   - Include code examples
   - Note any dependencies or requirements
   - Document props/variations if applicable

4. **Test before committing**
   - Open the component in multiple browsers
   - Verify responsive behavior
   - Check accessibility (keyboard navigation, screen readers)
   - Validate HTML and CSS

### Commit Guidelines

- Use clear, descriptive commit messages
- Format: `[Category] Brief description`
- Examples:
  - `[Buttons] Add primary CTA button component`
  - `[Forms] Create text input with validation states`
  - `[Docs] Update contribution guidelines`

### Pull Request Process

1. Create a feature branch: `git checkout -b feature/component-name`
2. Make your changes following the guidelines above
3. Test thoroughly
4. Commit with descriptive messages
5. Push and create a pull request
6. Request review from team members

## 📚 Documentation

Detailed documentation for each component can be found in:
- Component-specific READMEs in each component folder
- General guides in the `docs/` folder

## 🛠️ Tech Stack

- **HTML5**: Semantic markup
- **CSS3**: Modern CSS with custom properties
- **No frameworks**: Pure HTML/CSS for maximum flexibility
- **Google Fonts**: Lora and system fonts

## 📝 License

[Add your license information here]

## 👥 Team

[Add team member information here]

## 📞 Support

For questions or issues:
- Open an issue on GitHub
- Contact the design system team
- Check the documentation in `/docs`

---

**Last Updated**: January 2026
**Version**: 1.0.0
