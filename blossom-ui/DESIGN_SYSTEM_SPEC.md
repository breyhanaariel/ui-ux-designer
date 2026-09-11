# 🌸 Blossom UI — Design System Specification

## 1. Foundations

### Color
Build color as a layered token system.

**Primitive examples**
- `pink-50` → `pink-900`
- `lavender-50` → `lavender-900`
- `sage-50` → `sage-900`
- neutral scale

**Semantic examples**
- `surface/default`
- `surface/subtle`
- `text/primary`
- `text/secondary`
- `border/default`
- `action/primary`
- `status/success`
- `status/warning`
- `status/error`

Avoid tying component meaning directly to a decorative color name.

---

### Typography

Define roles rather than styling each screen independently.

Suggested roles:
- Display
- Heading XL
- Heading L
- Heading M
- Body
- Body Small
- Label
- Caption

Document:
- Font family
- Weight
- Size
- Line height
- Letter spacing
- Intended use

---

### Spacing

Use a consistent scale, for example:
`4 · 8 · 12 · 16 · 24 · 32 · 40 · 48 · 64`

Document which values are preferred for:
- Internal component padding
- Section spacing
- Page margins
- Dense vs. comfortable layouts

---

### Radius

Keep the system intentionally limited.

Example roles:
- `radius/small`
- `radius/medium`
- `radius/large`
- `radius/pill`

Use radius to reinforce hierarchy, not as decoration on every element.

---

### Elevation

Define a small scale for:
- Resting cards
- Hovered / raised content
- Dropdowns / menus
- Dialogs

Prefer borders and surface contrast where elevation is unnecessary.

---

## 2. Variables / Tokens

### Token layers

1. **Primitive** — raw values
2. **Semantic** — meaning-based aliases
3. **Component** — local component aliases where necessary

### Example

```
pink-600
   ↓
action-primary-bg
   ↓
button-primary-bg
```

This makes future theme changes safer than hard-coding pink directly into Button.

---

## 3. Responsive Layout

Define at least:
- Mobile
- Tablet
- Desktop

Document:
- Page gutters
- Content max-width
- Grid columns
- Component stacking behavior
- Navigation changes

Avoid calling a design system responsive unless these rules are demonstrated in actual screens.

---

## 4. Motion

Define a small set of durations:
- Fast feedback
- Standard transition
- Deliberate transition

Document:
- What may animate
- What should not animate
- Easing
- Reduced-motion alternatives

---

## 5. Content Style

Blossom's tone should feel:
- Warm
- Clear
- Reassuring
- Concise

Avoid using cute language where the user needs precise system feedback, especially for errors, destructive actions, permissions, or billing.

---

## 6. Example Product Application

Create at least one responsive web flow and one mobile flow entirely from Blossom components.

This section should eventually include:
- Component map
- Token usage
- Responsive comparison
- Accessibility annotations

📌 Visual slots are listed in [assets/README.md](./assets/README.md).
