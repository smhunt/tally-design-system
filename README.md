# Tally Design System

A minimal, clean design system inspired by Tally.so - CSS variables, components, and examples for modern web apps.

## 🤖 Claude Skill

This design system is available as a **Claude Skill**! Claude can help you build beautiful web interfaces using this design system.

- **Skill Name**: `tally-design-system`
- **Version**: 1.0.0
- **Type**: Design System

### Quick Start with Claude

Simply tell Claude:
> "Use the Tally Design System to create [your interface]"

Claude has access to all components, CSS variables, and best practices defined in this design system.

## 📦 What's Included

- **CSS Variables**: Complete design tokens for colors, typography, spacing, and more
- **UI Components**: Buttons, forms, cards, navigation, badges, and more
- **Utility Classes**: Flexbox helpers, spacing, and text utilities
- **Examples**: Ready-to-use component examples in `examples/index.html`

## 🚀 Installation

### Basic Usage

Include the design system in your HTML:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Your App</title>
    
    <!-- Google Fonts - Inter (recommended) -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&display=swap" rel="stylesheet">
    
    <!-- Tally Design System -->
    <link rel="stylesheet" href="css/tally-theme.css">
</head>
<body>
    <!-- Your content here -->
</body>
</html>
```

## 📚 Documentation

- **[Skill Instructions](SKILL_INSTRUCTIONS.md)**: Complete guide for Claude on using this design system
- **[Components Demo](examples/index.html)**: See all components in action
- **[CSS Variables](css/tally-theme.css)**: View all design tokens

## 🎨 Features

### Design Tokens
- Primary and accent colors (blue and pink)
- Comprehensive typography scale
- 4px-based spacing system
- Border radius variants
- Shadow system
- Smooth transitions

### Components
- **Buttons**: Primary, accent, secondary, ghost (with size variants)
- **Forms**: Inputs, textareas, labels
- **Cards**: Standard and hoverable cards
- **Navigation**: Sidebar navigation with sections
- **Badges**: Multiple badge styles
- **Toggle Switch**: Interactive on/off switch
- **Tabs**: Horizontal tab navigation
- **Avatar**: User avatar component
- **Header/Toolbar**: Page headers with breadcrumbs
- **Empty States**: Placeholder content areas

### Utility Classes
- Flexbox utilities
- Spacing helpers
- Text utilities
- Width utilities

## 🎯 Design Principles

1. **Minimal** - Clean, uncluttered interfaces
2. **Consistent** - Systematic design tokens and spacing
3. **Accessible** - Proper contrast and focus states
4. **Professional** - Business-focused aesthetic

## 📖 Usage Examples

### Simple Button
```html
<button class="tally-btn tally-btn-primary">Click Me</button>
```

### Form Input
```html
<label class="tally-label">Email</label>
<input type="email" class="tally-input" placeholder="your@email.com">
```

### Card Component
```html
<div class="tally-card">
    <div class="tally-card-title">Card Title</div>
    <div class="tally-card-description">Card description</div>
</div>
```

For more examples, see the [Skill Instructions](SKILL_INSTRUCTIONS.md) or explore `examples/index.html`.

## 🤝 Contributing

Contributions are welcome! Feel free to submit issues or pull requests.

## 📄 License

MIT License - feel free to use this design system in your projects.

## 🔗 Inspiration

Inspired by the clean, minimal design of [Tally.so](https://tally.so).
