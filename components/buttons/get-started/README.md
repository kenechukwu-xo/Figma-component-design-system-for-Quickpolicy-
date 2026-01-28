# Get Started Button

A primary call-to-action button with a purple gradient background, multiple shadow layers, and smooth hover effects.

## Preview

![Button Preview](preview.png)

## Features

- ✨ Multi-layer gradient background
- 🎨 Purple theme with light border
- 🌟 Elevation shadow system
- 🔄 Smooth hover and active states
- ♿ Accessible with focus states
- 📱 Responsive and flexible sizing

## Usage

### HTML

```html
<button class="btn-get-started">Get started</button>
```

### Required Files

1. **Design Tokens**: `styles/variables.css`
2. **Component Styles**: `components/buttons/get-started/get-started.css`
3. **Google Font**: Lora (Medium weight)

### Installation

#### Option 1: Link Stylesheet
```html
<!-- Include design tokens -->
<link rel="stylesheet" href="path/to/styles/variables.css">

<!-- Include component styles -->
<link rel="stylesheet" href="path/to/components/buttons/get-started/get-started.css">

<!-- Include Google Font -->
<link href="https://fonts.googleapis.com/css2?family=Lora:wght@500&display=swap" rel="stylesheet">
```

#### Option 2: Import in CSS
```css
@import url('path/to/styles/variables.css');
@import url('path/to/components/buttons/get-started/get-started.css');
```

## States

### Default
Standard button appearance with gradient and shadow.

### Hover
- Lifts up slightly (`translateY(-2px)`)
- Enhanced shadow for depth

### Active
- Returns to default position
- Standard shadow

### Focus
- Purple outline for accessibility
- 2px offset for visibility

### Disabled
- Reduced opacity (60%)
- No hover effects
- Not clickable

## Customization

You can customize the button by overriding CSS variables:

```css
.btn-get-started {
  /* Override design tokens */
  --primary-purple: rgb(100, 50, 200); /* Custom purple */
  --radius-xl: 16px; /* Adjust border radius */
  --font-size-xl: 18px; /* Change text size */
}
```

Or add custom classes:

```css
.btn-get-started.btn-large {
  padding: 16px 36px;
  font-size: 24px;
}

.btn-get-started.btn-small {
  padding: 8px 18px;
  font-size: 16px;
}
```

## Design Tokens Used

| Token | Value | Purpose |
|-------|-------|---------|
| `--primary-purple` | `rgb(147, 102, 221)` | Background base color |
| `--border-light-purple` | `#dccaf9` | Border color |
| `--text-white` | `#ffffff` | Text color |
| `--spacing-md` | `12px` | Vertical padding |
| `--radius-xl` | `20px` | Border radius |
| `--font-size-xl` | `20px` | Font size |
| `--shadow-button` | Multi-layer | Default elevation |
| `--shadow-button-hover` | Multi-layer | Hover elevation |

## Accessibility

- ✅ Keyboard navigable (Tab key)
- ✅ Focus indicator visible
- ✅ Disabled state properly marked
- ✅ Semantic `<button>` element
- ✅ Cursor indicates interactivity

### Recommendations
- Ensure sufficient color contrast (this button meets WCAG AA standards)
- Add `aria-label` if button text is not descriptive enough
- Test with screen readers

## Browser Support

- ✅ Chrome/Edge (latest)
- ✅ Firefox (latest)
- ✅ Safari (latest)
- ✅ Mobile browsers

## Examples

### Basic Usage
```html
<button class="btn-get-started">Get started</button>
```

### With Icon
```html
<button class="btn-get-started">
  <svg width="20" height="20" style="margin-right: 8px;">...</svg>
  Get started
</button>
```

### As Link
```html
<a href="/signup" class="btn-get-started" role="button">Get started</a>
```

## Notes

- The button uses inline SVG data URIs for gradient effects
- Gradient IDs are unique to avoid conflicts with multiple buttons
- Font loading may cause a brief flash if not preloaded

## Figma Source

- **File**: NETHERMIND-DESIGN-TASK-Kenechukwu
- **Node ID**: 3031:1341
- **Last Updated**: January 2026

---

For issues or questions, refer to the main repository README.
