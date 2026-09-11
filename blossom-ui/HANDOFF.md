# 💻 Blossom UI — Developer Handoff

## 🌷 Goal

Create a Figma structure that maps cleanly to implementation rather than requiring developers to reinterpret visual intent.

---

## 1. Naming

Use predictable naming.

Examples:
```
Button / Primary
Button / Secondary
Input / Text
Input / Select
Feedback / Toast
Overlay / Dialog
```

Token examples:
```
color.surface.default
color.text.primary
color.action.primary
space.200
radius.md
shadow.overlay
motion.duration.fast
```

---

## 2. Figma Properties → Code Props

Example mapping:

| Figma | Possible Code |
|---|---|
| Variant = Primary | `variant="primary"` |
| Size = Medium | `size="md"` |
| Disabled = True | `disabled` |
| Loading = True | `loading` |
| Icon = Leading | `startIcon` |

The exact API is illustrative; final implementation should be agreed with engineering.

---

## 3. Handoff Notes Per Component

Document:
- Usage
- Anatomy
- Variants
- States
- Dimensions
- Responsive behavior
- Content constraints
- Motion
- Accessibility
- Edge cases

---

## 4. Required Edge Cases

Designers should expose:
- Long labels
- Validation errors
- Empty data
- Loading
- Offline / failure
- Disabled states
- Destructive confirmation
- Small viewport behavior

A component isn't fully specified if only its ideal state exists.

---

## 5. Storybook Parity

A future implementation could mirror Blossom UI's component hierarchy in Storybook.

For the portfolio, demonstrate the intended mapping with at least one component:

`Figma component → properties → states → accessibility notes → Storybook-style documentation mockup`

📌 Suggested export: `assets/09-handoff-spec.png`

---

## 6. Definition of Ready

A component is ready for handoff when:
- [ ] Design tokens are used
- [ ] Supported variants are defined
- [ ] Interactive states exist
- [ ] Responsive behavior is known
- [ ] Accessibility behavior is documented
- [ ] Edge cases are represented
- [ ] Naming is consistent
- [ ] Usage guidance exists
