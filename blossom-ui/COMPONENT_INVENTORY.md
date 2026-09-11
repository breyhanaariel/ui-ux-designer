# 🌷 Blossom UI — Component Inventory

> Build depth before breadth. A smaller set of fully specified components is more convincing than dozens of decorative ones.

## 🌼 Tier 1 — Portfolio Minimum

### Actions
- Button
- Icon Button
- Link

### Inputs
- Text Field
- Text Area
- Select
- Checkbox
- Radio
- Switch

### Navigation
- Tabs
- Breadcrumbs
- Top Navigation
- Mobile Navigation

### Feedback
- Alert
- Toast
- Progress / Spinner
- Tooltip

### Overlays
- Dialog
- Popover / Menu

### Content
- Card
- Badge
- Avatar
- Divider

---

## 🌸 Required Component Documentation

For each major component document:

### Anatomy
What are the component's parts?

### Variants
Example: primary / secondary / tertiary / destructive

### Sizes
Only include sizes with a real product need.

### States
- Default
- Hover
- Focus
- Pressed
- Disabled
- Loading
- Error where relevant

### Responsive behavior
What changes at smaller widths?

### Accessibility
- Keyboard behavior
- Focus behavior
- Accessible name
- Error association
- Target size

### Content guidance
What text belongs here? What should be avoided?

### Do / Don't
Show misuse as well as correct use.

### Developer mapping
Map Figma props/variants to likely implementation props.

---

## 🌺 Suggested Figma Property Pattern

For a Button:

```
Variant = Primary | Secondary | Tertiary | Destructive
Size = Small | Medium | Large
State = Default | Hover | Pressed | Focus | Disabled
Icon = None | Leading | Trailing | IconOnly
Loading = True | False
```

Avoid creating every theoretical combination if it has no product use.

---

## 🩰 Pattern-Level Examples

Once Tier 1 components exist, create:
- Sign-in form
- Settings form
- Confirmation dialog
- Empty state
- Error state
- Success feedback
- Responsive navigation pattern

These prove that components work together as a system.
