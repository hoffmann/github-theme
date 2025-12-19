# GitHub Theme

A simple, clean, and responsive CSS theme inspired by GitHub's design language. Perfect for building modern web applications and documentation sites.

## Features

- **GitHub-inspired Design** - Clean, professional aesthetics matching GitHub's visual language
- **Responsive Grid System** - 12-column flexible grid with mobile-first breakpoints
- **Complete Component Library** - Buttons, forms, alerts, badges, navigation, and more
- **Flexbox Utilities** - Comprehensive flexbox classes for modern layouts
- **Utility Classes** - Spacing, typography, and display utilities for rapid development
- **GitHub Markdown Styles** - Official GitHub markdown CSS for rich text content
- **CSS Variables** - Easy theming and customization
- **Lightweight** - No JavaScript dependencies, pure CSS

## Quick Start

### 1. Include the CSS Files

```html
<link rel="stylesheet" href="css/style.css">
<link rel="stylesheet" href="css/github-markdown-light.css">
```

### 2. Use the Components

```html
<div class="container">
  <button class="btn btn-primary">Click Me</button>

  <div class="alert alert-success">
    <strong>Success!</strong> Your action was completed.
  </div>

  <div class="markdown-body">
    <h1>Your Content</h1>
    <p>Styled with GitHub markdown CSS.</p>
  </div>
</div>
```

### 3. Build Responsive Layouts

```html
<div class="container">
  <div class="row">
    <div class="col-12 col-md-6">Column 1</div>
    <div class="col-12 col-md-6">Column 2</div>
  </div>
</div>
```

## Documentation & Examples

### Core Components

- **[Buttons](example-buttons.html)** - Multiple button variants, sizes, and states
- **[Alerts](example-alerts.html)** - Contextual feedback messages (info, success, warning, danger)
- **[Badges](example-badges.html)** - Small labels and status indicators
- **[Forms](example-forms.html)** - Styled form controls and layouts
- **[Navigation](example-navigation.html)** - Nav bars, tabs, breadcrumbs, and pagination

### Layout System

- **[Grid System](example-grid.html)** - 12-column responsive grid with breakpoints
- **[Flexbox Utilities](example-flexbox.html)** - Complete flexbox layout utilities

### Styling

- **[Markdown Styling](example-markdown.html)** - GitHub markdown CSS for rich text
- **[Utility Classes](example-utilities.html)** - Spacing, text, and display utilities

## Component Overview

### Buttons

```html
<button class="btn btn-primary">Primary</button>
<button class="btn btn-secondary">Secondary</button>
<button class="btn btn-success">Success</button>
<button class="btn btn-danger">Danger</button>
<button class="btn btn-outline">Outline</button>
```

**Sizes:** `.btn-sm`, `.btn-lg`, `.btn-block`

### Alerts

```html
<div class="alert alert-info">Info message</div>
<div class="alert alert-success">Success message</div>
<div class="alert alert-warning">Warning message</div>
<div class="alert alert-danger">Error message</div>
```

### Badges

```html
<span class="badge badge-primary">Primary</span>
<span class="badge badge-success">Success</span>
<span class="badge badge-danger">Danger</span>
<span class="badge badge-secondary">Secondary</span>
```

### Cards

```html
<div class="card">
  <h3 class="card-header">Card Title</h3>
  <div class="card-body">
    <p>Card content goes here.</p>
  </div>
  <div class="card-footer">Footer text</div>
</div>
```

### Forms

```html
<div class="form-group">
  <label class="form-label" for="email">Email</label>
  <input type="email" class="form-control" id="email" placeholder="your@email.com">
</div>
```

## Grid System

The grid uses a 12-column layout with responsive breakpoints:

- **Small (sm):** ≥576px
- **Medium (md):** ≥768px
- **Large (lg):** ≥1024px

### Basic Grid

```html
<div class="row">
  <div class="col-6">50% width</div>
  <div class="col-6">50% width</div>
</div>
```

### Responsive Grid

```html
<div class="row">
  <div class="col-12 col-md-4">Full width on mobile, 33% on tablet+</div>
  <div class="col-12 col-md-4">Full width on mobile, 33% on tablet+</div>
  <div class="col-12 col-md-4">Full width on mobile, 33% on tablet+</div>
</div>
```

## Flexbox Utilities

### Display Flex

```html
<div class="d-flex">
  <div>Item 1</div>
  <div>Item 2</div>
</div>
```

### Justify Content

- `.justify-content-start` - Align items to start
- `.justify-content-end` - Align items to end
- `.justify-content-center` - Center items
- `.justify-content-between` - Space between items
- `.justify-content-around` - Space around items

### Align Items

- `.align-items-start` - Align to start of cross axis
- `.align-items-end` - Align to end of cross axis
- `.align-items-center` - Center on cross axis
- `.align-items-baseline` - Align by baseline
- `.align-items-stretch` - Stretch to fill container

### Flex Direction

- `.flex-row` - Horizontal direction (default)
- `.flex-column` - Vertical direction

## Utility Classes

### Spacing (8px base unit)

**Margin:**
- `.mt-*` - Margin top (0-5)
- `.mb-*` - Margin bottom (0-5)

**Padding:**
- `.pt-*` - Padding top (0-5)
- `.pb-*` - Padding bottom (0-5)

### Text Alignment

- `.text-left` - Left align
- `.text-center` - Center align
- `.text-right` - Right align

### Text Colors

- `.text-muted` - Muted/secondary text
- `.text-primary` - Primary brand color
- `.text-success` - Success color
- `.text-danger` - Danger color

### Display

- `.d-none` - Hide element
- `.d-block` - Display as block
- `.d-inline` - Display inline
- `.d-inline-block` - Display inline-block
- `.d-flex` - Enable flexbox

### Responsive Display

- `.d-sm-*` - Applies at 576px+
- `.d-md-*` - Applies at 768px+
- `.d-lg-*` - Applies at 1024px+

## Customization

The theme uses CSS variables for easy customization:

```css
:root {
  --color-primary: #0969da;
  --color-success: #1a7f37;
  --color-danger: #cf222e;
  --color-text: #1f2328;
  --color-bg: #ffffff;
  --border-radius: 6px;
  --spacing-unit: 8px;
}
```

## Container Sizes

- `.container` - Default container (max-width: 1280px)
- `.container-sm` - Small container (max-width: 768px)
- `.container-lg` - Large container (max-width: 1400px)

## Markdown Styling

Use the `.markdown-body` class to apply GitHub's markdown styles:

```html
<div class="markdown-body">
  <h1>Heading</h1>
  <p>Paragraph with <strong>bold</strong> and <em>italic</em> text.</p>
  <pre><code>Code block</code></pre>
  <blockquote>Blockquote</blockquote>
  <table>
    <thead><tr><th>Header</th></tr></thead>
    <tbody><tr><td>Data</td></tr></tbody>
  </table>
</div>
```

## Browser Support

- Chrome 90+
- Firefox 88+
- Safari 14+
- Edge 90+

## Best Practices

1. **Mobile-First:** Start with mobile styles, add responsive classes for larger screens
2. **Use Semantic HTML:** Choose appropriate HTML elements before adding classes
3. **Combine Utilities:** Mix utility classes with components for precise control
4. **Consistent Spacing:** Use the spacing scale (0-5) for visual consistency
5. **Accessible Forms:** Always use labels with form inputs
6. **Test Responsively:** Check layouts at all breakpoints

## File Structure

```
github-theme/
├── css/
│   ├── style.css                    # Main theme styles
│   └── github-markdown-light.css    # GitHub markdown styles
├── example-buttons.html             # Button examples
├── example-alerts.html              # Alert examples
├── example-badges.html              # Badge examples
├── example-forms.html               # Form examples
├── example-navigation.html          # Navigation examples
├── example-grid.html                # Grid system examples
├── example-flexbox.html             # Flexbox utility examples
├── example-markdown.html            # Markdown styling examples
├── example-utilities.html           # Utility class examples
└── index.md                         # This file
```

## License

MIT License - Feel free to use in your projects.

## Credits

- Markdown styles from [GitHub's official markdown CSS](https://github.com/sindresorhus/github-markdown-css)
- Design inspired by GitHub's interface
- Built with modern CSS (Flexbox, CSS Variables)

---

**Get Started:** Browse the [example files](example-buttons.html) to see all components in action!
