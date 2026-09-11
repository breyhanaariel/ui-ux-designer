# ♿ Blossom UI — Accessibility Guidelines

Blossom UI should be **designed and evaluated against relevant WCAG 2.2 AA criteria**. This document is guidance for design and handoff; it is not a certification claim.

---

## 🌷 Color

- Verify text contrast for every semantic text role.
- Verify non-text contrast for controls, focus indicators, and meaningful boundaries.
- Do not use pastel color alone to communicate status.
- Provide icons, labels, or patterns for success/error/warning states.

---

## 🌼 Focus

Interactive components should specify:
- Visible keyboard focus state
- Focus order expectations
- Focus trapping for modal dialogs
- Focus return behavior after overlays close

The decorative floral aesthetic must never obscure focus visibility.

---

## 🌸 Forms

Every control needs:
- Persistent label where appropriate
- Accessible name
- Clear required/optional treatment
- Error message
- Error association in implementation
- Help text when necessary

Placeholder text should not be the only label.

---

## 🌺 Target Size

Design touch targets with comfortable interaction areas. Small icons may visually remain compact while receiving a larger hit area.

---

## 🩰 Motion

Document reduced-motion alternatives.

Decorative:
- Sparkles
- Bounces
- Large transforms

should be removable without losing meaning.

Functional state changes must still be understandable without animation.

---

## 🌹 Status & Feedback

Never rely on:
- Pink = error
- Green = success
- Animation = complete

Pair visual styling with text and/or icons.

---

## 💻 Handoff Notes

For components that require semantics, specify intended implementation behavior.

Examples:
- Dialog → modal semantics + focus management
- Tooltip → supplemental description, not essential content
- Switch → binary on/off state
- Tabs → keyboard-navigation expectations
- Error text → programmatically associated with its field

---

## ✅ Review Checklist

Before calling a component complete:
- [ ] Contrast reviewed
- [ ] Focus state exists
- [ ] Keyboard behavior documented
- [ ] Target size reviewed
- [ ] Status is not color-only
- [ ] Error behavior exists
- [ ] Reduced-motion behavior considered
- [ ] Accessible name / semantics noted
