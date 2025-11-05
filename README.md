# Accessible Periodic Table

An accessible and WCAG 2.1 AA compliant periodic table of elements built with HTML, CSS, and JavaScript.

## Features

### Accessibility Compliance

This periodic table meets WCAG 2.1 Level AA standards and includes:

#### 1. **Keyboard Navigation**
- Full keyboard support with Tab navigation
- Arrow keys for grid-style navigation (up, down, left, right)
- Enter/Space to activate elements and view details
- Escape key to close modal dialogs
- Visible focus indicators on all interactive elements

#### 2. **Screen Reader Support**
- Semantic HTML structure with proper ARIA labels
- Descriptive `aria-label` attributes on each element containing:
  - Element name
  - Atomic number
  - Atomic mass
  - Category classification
- Role attributes (`role="grid"`, `role="gridcell"`, `role="dialog"`)
- Skip-to-content link for keyboard users
- Modal dialogs with `aria-modal` and `aria-labelledby`

#### 3. **Visual Accessibility**
- WCAG AA compliant color contrast ratios (minimum 4.5:1 for normal text, 3:1 for large text)
- Clear visual focus indicators with 3px outline
- Color-coded categories with accompanying text labels in legend
- High contrast mode support via media queries
- Responsive design that works at different zoom levels

#### 4. **Reduced Motion Support**
- `prefers-reduced-motion` media query disables animations for users with motion sensitivity

#### 5. **Semantic HTML**
- Proper heading hierarchy (`<h1>`, `<h2>`)
- Semantic elements (`<header>`, `<main>`, `<nav>`)
- Button elements for interactive components
- Proper landmark regions

## Usage

### Opening the Periodic Table

Simply open `index.html` in a modern web browser:

```bash
open index.html
```

Or use a local server:

```bash
python -m http.server 8000
# Then navigate to http://localhost:8000
```

### Keyboard Controls

- **Tab**: Navigate between elements
- **Shift + Tab**: Navigate backwards
- **Arrow Keys**: Navigate in grid pattern (up/down/left/right)
- **Enter or Space**: Open element details modal
- **Escape**: Close modal dialog

### Interactive Features

- Click or press Enter on any element to view detailed information
- Color-coded categories help identify element types
- Hover effects provide visual feedback
- Modal dialogs display additional element information

## WCAG 2.1 Compliance Checklist

- ✅ **1.1.1 Non-text Content**: All non-text content has text alternatives
- ✅ **1.3.1 Info and Relationships**: Information structure is programmatically determined
- ✅ **1.4.3 Contrast (Minimum)**: Color contrast ratio meets AA standards
- ✅ **2.1.1 Keyboard**: All functionality available via keyboard
- ✅ **2.1.2 No Keyboard Trap**: Keyboard focus can move away from components
- ✅ **2.4.1 Bypass Blocks**: Skip link provided
- ✅ **2.4.3 Focus Order**: Focus order is logical and intuitive
- ✅ **2.4.7 Focus Visible**: Keyboard focus indicator is visible
- ✅ **3.2.1 On Focus**: No unexpected context changes on focus
- ✅ **4.1.2 Name, Role, Value**: All UI components have accessible names and roles
- ✅ **4.1.3 Status Messages**: Status changes are announced to screen readers

## Browser Support

- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)
- Screen readers: NVDA, JAWS, VoiceOver

## Technologies Used

- HTML5
- CSS3 (Grid Layout, Custom Properties)
- Vanilla JavaScript (ES6+)
- ARIA (Accessible Rich Internet Applications)

## License

MIT License
