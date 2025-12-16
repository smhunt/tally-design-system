# Tally Design System - Claude Skill Instructions

## Overview
The Tally Design System is a minimal, clean design system inspired by Tally.so. It provides CSS variables, pre-built components, and utility classes for building modern web applications with a consistent, professional look.

## Installation & Setup

### Basic Usage
Include the Tally Design System in your HTML:

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

## Design Tokens (CSS Variables)

### Colors

#### Primary Colors
- `--tally-primary: #0070D7` - Main brand blue
- `--tally-primary-hover: #0060B8` - Hover state for primary
- `--tally-primary-light: rgba(0, 112, 215, 0.1)` - Light background for focus states

#### Accent Colors (Pink/Magenta)
- `--tally-accent: #E91E8C` - Accent pink/magenta
- `--tally-accent-hover: #D01A7E` - Hover state for accent
- `--tally-accent-light: #FFE4F3` - Light pink background

#### Neutral Colors
- `--tally-white: #FFFFFF`
- `--tally-background: #FFFFFF` - Page background
- `--tally-surface: #FFFFFF` - Card/component background
- `--tally-text-primary: #000000` - Main text color
- `--tally-text-secondary: #37352F` - Secondary text
- `--tally-text-muted: #6B6B6B` - Muted/disabled text
- `--tally-placeholder: #BBBAB8` - Input placeholder text

#### Border Colors
- `--tally-border: #E5E5E5` - Standard border
- `--tally-border-input: #3D3B3B` - Input border
- `--tally-border-light: #F0F0F0` - Light border

#### Status Colors
- `--tally-upgrade: #E5A800` - Upgrade/premium features
- `--tally-upgrade-light: #FFF8E1` - Light upgrade background
- `--tally-success: #00C853` - Success state
- `--tally-error: #FF4444` - Error state

#### Sidebar
- `--tally-sidebar-bg: #FFFFFF`
- `--tally-sidebar-hover: #F5F5F5`
- `--tally-sidebar-active: #F0F0F0`

### Typography

#### Font Family
- `--tally-font-family: 'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, sans-serif`

#### Font Sizes
- `--tally-text-xs: 12px`
- `--tally-text-sm: 14px`
- `--tally-text-base: 16px`
- `--tally-text-lg: 18px`
- `--tally-text-xl: 20px`
- `--tally-text-2xl: 24px`
- `--tally-text-3xl: 30px`
- `--tally-text-4xl: 36px`
- `--tally-text-5xl: 48px`

#### Font Weights
- `--tally-font-normal: 400`
- `--tally-font-medium: 500`
- `--tally-font-semibold: 600`
- `--tally-font-bold: 700`

#### Line Heights
- `--tally-leading-tight: 1.25` - For headings
- `--tally-leading-normal: 1.5` - For body text
- `--tally-leading-relaxed: 1.625` - For comfortable reading

### Spacing
- `--tally-space-1: 4px`
- `--tally-space-2: 8px`
- `--tally-space-3: 12px`
- `--tally-space-4: 16px`
- `--tally-space-5: 20px`
- `--tally-space-6: 24px`
- `--tally-space-8: 32px`
- `--tally-space-10: 40px`
- `--tally-space-12: 48px`
- `--tally-space-16: 64px`

### Border Radius
- `--tally-radius-sm: 4px`
- `--tally-radius-md: 8px`
- `--tally-radius-lg: 12px`
- `--tally-radius-xl: 16px`
- `--tally-radius-full: 9999px` - Fully rounded (pills, avatars)

### Shadows
- `--tally-shadow-sm: 0 1px 2px rgba(0, 0, 0, 0.05)` - Subtle shadow
- `--tally-shadow-md: 0 4px 6px rgba(0, 0, 0, 0.07)` - Medium shadow
- `--tally-shadow-lg: 0 10px 15px rgba(0, 0, 0, 0.1)` - Large shadow
- `--tally-shadow-card: 0 1px 3px rgba(0, 0, 0, 0.08)` - Card shadow

### Transitions
- `--tally-transition-fast: 0.15s ease` - Quick interactions
- `--tally-transition-normal: 0.2s ease` - Standard animations
- `--tally-transition-slow: 0.3s ease` - Slower, smoother transitions

## Components

### Buttons

#### Basic Button Structure
```html
<button class="tally-btn tally-btn-primary">Primary Button</button>
```

#### Button Variants

**Primary Button** (Blue):
```html
<button class="tally-btn tally-btn-primary">Primary Action</button>
```

**Accent Button** (Pink):
```html
<button class="tally-btn tally-btn-accent">Accent Action</button>
```

**Secondary/Outline Button**:
```html
<button class="tally-btn tally-btn-secondary">Secondary Action</button>
```

**Ghost Button** (Transparent):
```html
<button class="tally-btn tally-btn-ghost">Ghost Action</button>
```

#### Button Sizes
```html
<button class="tally-btn tally-btn-primary tally-btn-sm">Small</button>
<button class="tally-btn tally-btn-primary">Default</button>
<button class="tally-btn tally-btn-primary tally-btn-lg">Large</button>
```

#### Buttons with Icons
```html
<button class="tally-btn tally-btn-primary">
    <svg><!-- Icon here --></svg>
    Button with Icon
</button>
```

### Form Inputs

#### Text Input
```html
<label class="tally-label">Email Address</label>
<input type="email" class="tally-input" placeholder="Enter your email">
```

#### Textarea
```html
<label class="tally-label">Message</label>
<textarea class="tally-input tally-textarea" placeholder="Enter your message"></textarea>
```

#### Disabled Input
```html
<input type="text" class="tally-input" disabled value="Disabled input">
```

### Cards

#### Basic Card
```html
<div class="tally-card">
    <div class="tally-card-title">Card Title</div>
    <div class="tally-card-description">Card description goes here</div>
</div>
```

#### Hoverable Card
```html
<div class="tally-card tally-card-hover">
    <div class="tally-card-title">Interactive Card</div>
    <div class="tally-card-description">This card has hover effects</div>
</div>
```

### Sidebar Navigation

#### Sidebar Structure
```html
<aside class="tally-sidebar">
    <div class="tally-sidebar-section">
        <div class="tally-sidebar-title">Workspace</div>
        <a href="#" class="tally-sidebar-item active">
            Dashboard
        </a>
        <a href="#" class="tally-sidebar-item">
            Forms
        </a>
        <a href="#" class="tally-sidebar-item">
            Responses
        </a>
    </div>
    
    <div class="tally-sidebar-section">
        <div class="tally-sidebar-title">Account</div>
        <a href="#" class="tally-sidebar-item">
            Settings
        </a>
        <a href="#" class="tally-sidebar-item tally-sidebar-item-upgrade">
            Upgrade
        </a>
    </div>
</aside>
```

### Badges / Pills

#### Badge Variants
```html
<span class="tally-badge tally-badge-primary">Primary</span>
<span class="tally-badge tally-badge-accent">Accent</span>
<span class="tally-badge tally-badge-outline">Outline</span>
<span class="tally-badge tally-badge-upgrade">Upgrade</span>
<span class="tally-badge tally-badge-success">Success</span>
```

### Toggle Switch

```html
<div class="tally-toggle" onclick="this.classList.toggle('active')">
    <div class="tally-toggle-knob"></div>
</div>
```

With JavaScript:
```javascript
const toggle = document.querySelector('.tally-toggle');
toggle.addEventListener('click', () => {
    toggle.classList.toggle('active');
});
```

### Tabs

```html
<div class="tally-tabs">
    <button class="tally-tab active">Overview</button>
    <button class="tally-tab">Analytics</button>
    <button class="tally-tab">Settings</button>
</div>
```

### Avatar

```html
<!-- Default Avatar -->
<div class="tally-avatar">JD</div>

<!-- Small Avatar -->
<div class="tally-avatar tally-avatar-sm">JD</div>

<!-- Large Avatar -->
<div class="tally-avatar tally-avatar-lg">JD</div>
```

### Header / Toolbar

```html
<header class="tally-header">
    <div class="tally-breadcrumb">
        <a href="#" class="tally-breadcrumb-item">Home</a>
        <span class="tally-breadcrumb-separator">/</span>
        <a href="#" class="tally-breadcrumb-item">Forms</a>
        <span class="tally-breadcrumb-separator">/</span>
        <span class="tally-breadcrumb-item">Contact Form</span>
    </div>
    
    <div class="tally-flex tally-gap-3 tally-items-center">
        <button class="tally-btn tally-btn-secondary">Preview</button>
        <button class="tally-btn tally-btn-primary">Publish</button>
    </div>
</header>
```

### Empty State

```html
<div class="tally-empty-state">
    <div class="tally-empty-state-title">No forms yet</div>
    <div class="tally-empty-state-description">
        Get started by creating your first form
    </div>
    <button class="tally-btn tally-btn-primary">Create Form</button>
</div>
```

## Utility Classes

### Flexbox
- `.tally-flex` - Display flex
- `.tally-flex-col` - Flex direction column
- `.tally-items-center` - Align items center
- `.tally-justify-center` - Justify content center
- `.tally-justify-between` - Justify content space-between
- `.tally-gap-1`, `.tally-gap-2`, `.tally-gap-3`, `.tally-gap-4` - Gap spacing

### Spacing
- `.tally-m-0` - Margin 0
- `.tally-mt-4` - Margin top 16px
- `.tally-mb-4` - Margin bottom 16px
- `.tally-p-4` - Padding 16px
- `.tally-p-6` - Padding 24px

### Text
- `.tally-text-sm` - Small text (14px)
- `.tally-text-center` - Text align center
- `.tally-text-accent` - Accent color text
- `.tally-text-muted` - Muted color text
- `.tally-font-medium` - Medium font weight (500)
- `.tally-font-bold` - Bold font weight (700)

### Width
- `.tally-w-full` - Width 100%

## Typography Styles

### Headings
All headings have zero margin by default and use tight line-height:

```html
<h1>Heading 1</h1> <!-- 36px, bold -->
<h2>Heading 2</h2> <!-- 30px, bold -->
<h3>Heading 3</h3> <!-- 24px, semibold -->
<h4>Heading 4</h4> <!-- 20px, semibold -->
<h5>Heading 5</h5> <!-- 18px, medium -->
<h6>Heading 6</h6> <!-- 16px, medium -->
```

### Paragraphs
```html
<p>Body text uses secondary color (#37352F) and has bottom margin of 16px</p>
```

### Links
```html
<a href="#">Links use primary color and underline on hover</a>
```

## Best Practices for Claude

### When to Use This Design System
1. Building web applications with a clean, modern aesthetic
2. Creating forms and data collection interfaces
3. Developing dashboard and admin interfaces
4. Building minimal, focused landing pages
5. Creating SaaS product interfaces

### Design Principles
1. **Minimal** - Use clean, uncluttered layouts
2. **Consistent** - Stick to the defined spacing and color scales
3. **Accessible** - Ensure proper contrast and focus states
4. **Professional** - Maintain the clean, business-focused aesthetic

### Component Composition
Combine components to create complex interfaces:

```html
<div class="tally-card">
    <div class="tally-flex tally-justify-between tally-items-center tally-mb-4">
        <h3>Settings</h3>
        <span class="tally-badge tally-badge-primary">Pro</span>
    </div>
    
    <div class="tally-flex tally-flex-col tally-gap-4">
        <div>
            <label class="tally-label">Name</label>
            <input type="text" class="tally-input" placeholder="Enter your name">
        </div>
        
        <div>
            <label class="tally-label">Email</label>
            <input type="email" class="tally-input" placeholder="Enter your email">
        </div>
        
        <div class="tally-flex tally-justify-between tally-items-center">
            <span class="tally-text-sm">Email notifications</span>
            <div class="tally-toggle active">
                <div class="tally-toggle-knob"></div>
            </div>
        </div>
        
        <div class="tally-flex tally-gap-3">
            <button class="tally-btn tally-btn-secondary">Cancel</button>
            <button class="tally-btn tally-btn-primary">Save Changes</button>
        </div>
    </div>
</div>
```

### Color Usage Guidelines
- **Primary Blue** (`--tally-primary`): Main CTAs, links, focus states
- **Accent Pink** (`--tally-accent`): Secondary CTAs, highlights, special features
- **Neutral Colors**: Text hierarchy (primary → secondary → muted)
- **Status Colors**: Success messages, upgrade prompts, errors

### Spacing Scale
Follow the 4px base spacing scale for consistency:
- Use `--tally-space-2` (8px) for tight spacing
- Use `--tally-space-4` (16px) for standard spacing
- Use `--tally-space-6` (24px) for section spacing
- Use `--tally-space-8` (32px) or larger for page-level spacing

### Responsive Considerations
While the design system doesn't include responsive utilities, follow these guidelines:
- Use viewport units or percentages for flexible layouts
- Stack components vertically on mobile using flexbox
- Reduce padding/margins on smaller screens
- Consider hiding sidebar on mobile, using a hamburger menu instead

## Example Layouts

### Simple Form Page
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Contact Form</title>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="css/tally-theme.css">
</head>
<body style="display: flex; align-items: center; justify-content: center; min-height: 100vh; background-color: var(--tally-background);">
    <div class="tally-card" style="max-width: 500px; width: 100%;">
        <h2 class="tally-mb-4">Contact Us</h2>
        <p class="tally-text-muted tally-mb-4">Send us a message and we'll get back to you soon.</p>
        
        <form class="tally-flex tally-flex-col tally-gap-4">
            <div>
                <label class="tally-label">Name</label>
                <input type="text" class="tally-input" placeholder="Your name" required>
            </div>
            
            <div>
                <label class="tally-label">Email</label>
                <input type="email" class="tally-input" placeholder="your@email.com" required>
            </div>
            
            <div>
                <label class="tally-label">Message</label>
                <textarea class="tally-input tally-textarea" placeholder="How can we help?" required></textarea>
            </div>
            
            <button type="submit" class="tally-btn tally-btn-primary tally-w-full">Send Message</button>
        </form>
    </div>
</body>
</html>
```

### Dashboard Layout
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Dashboard</title>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="css/tally-theme.css">
    <style>
        .layout {
            display: flex;
            height: 100vh;
        }
        .main {
            flex: 1;
            display: flex;
            flex-direction: column;
            overflow: hidden;
        }
        .content {
            flex: 1;
            overflow-y: auto;
            padding: var(--tally-space-8);
        }
    </style>
</head>
<body>
    <div class="layout">
        <aside class="tally-sidebar">
            <div class="tally-sidebar-section">
                <div class="tally-sidebar-title">Workspace</div>
                <a href="#" class="tally-sidebar-item active">Dashboard</a>
                <a href="#" class="tally-sidebar-item">Forms</a>
                <a href="#" class="tally-sidebar-item">Responses</a>
            </div>
            <div class="tally-sidebar-section">
                <div class="tally-sidebar-title">Account</div>
                <a href="#" class="tally-sidebar-item">Settings</a>
                <a href="#" class="tally-sidebar-item tally-sidebar-item-upgrade">Upgrade</a>
            </div>
        </aside>
        
        <main class="main">
            <header class="tally-header">
                <h3>Dashboard</h3>
                <div class="tally-flex tally-gap-3 tally-items-center">
                    <button class="tally-btn tally-btn-secondary tally-btn-sm">Export</button>
                    <button class="tally-btn tally-btn-primary tally-btn-sm">Create Form</button>
                    <div class="tally-avatar">JD</div>
                </div>
            </header>
            
            <div class="content">
                <div class="tally-flex tally-gap-4" style="flex-wrap: wrap;">
                    <div class="tally-card" style="flex: 1; min-width: 250px;">
                        <div class="tally-card-title">Total Forms</div>
                        <div class="tally-card-description">24</div>
                    </div>
                    <div class="tally-card" style="flex: 1; min-width: 250px;">
                        <div class="tally-card-title">Responses</div>
                        <div class="tally-card-description">1,234</div>
                    </div>
                    <div class="tally-card" style="flex: 1; min-width: 250px;">
                        <div class="tally-card-title">Conversion</div>
                        <div class="tally-card-description">67%</div>
                    </div>
                </div>
            </div>
        </main>
    </div>
</body>
</html>
```

## Tips for Claude

1. **Always include the font link**: The design system looks best with the Inter font from Google Fonts
2. **Use CSS variables for custom styling**: Extend the design system by referencing existing variables
3. **Combine utility classes**: Use utility classes like `tally-flex`, `tally-gap-4`, etc., for quick layouts
4. **Follow the spacing scale**: Stick to the defined spacing scale (4px increments)
5. **Maintain consistency**: Use the same color variables throughout an interface
6. **Consider states**: Remember to handle hover, focus, active, and disabled states
7. **Keep it minimal**: The design system emphasizes clean, uncluttered interfaces
8. **Test accessibility**: Ensure proper color contrast and keyboard navigation

## Version
This skill documentation is for Tally Design System v1.0.0
