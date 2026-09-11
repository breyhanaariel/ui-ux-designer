# ♿ Honeycomb HQ — Accessibility Specification

Honeycomb HQ should be **designed and evaluated against relevant WCAG 2.2 AA criteria**. This is a design/prototype target, not a certification claim.

---

## 🌼 Information & Status

Complex business UI must not depend on color alone.

For:
- Project health
- Invoice status
- Approval status
- Capacity warnings

use readable text labels plus color/icon treatment.

---

## ⌨️ Keyboard

Primary flows should be usable without a pointer.

Test:
- Navigation
- Search
- Filters
- Tables / list actions
- Forms
- Menus
- Dialogs
- Tabs
- Approval actions

---

## 🔎 Focus

- Strong visible focus indicator
- Focus not clipped by containers
- Logical order
- Dialog focus trap
- Return focus to trigger after close
- New validation errors receive appropriate attention without disorienting users

---

## 📊 Data Tables

Desktop semantic tables should have:
- Column headers
- Appropriate scope/relationships
- Accessible sorting state
- Row action labels that identify the target

Responsive card transformations should preserve labels for values.

---

## 📝 Forms

- Programmatic labels
- Instructions before errors where possible
- Error association
- Required state
- Status announcements for async mock actions
- No placeholder-only labels

---

## 🪟 Dialogs & Menus

Dialogs:
- Accessible name
- Modal semantics
- Initial focus
- Escape behavior
- Return focus

Menus:
- Predictable keyboard interaction
- Clear trigger labels
- No hover-only access

---

## 🔠 Zoom / Reflow

Test prototype at:
- 200% zoom
- Narrow desktop viewport
- Mobile widths

Critical controls must remain usable without two-dimensional scrolling except where data itself reasonably requires it.

---

## 🎞️ Motion

Respect `prefers-reduced-motion`.

Reduced-motion mode should:
- Remove decorative transforms
- Shorten/disable nonessential animation
- Preserve visible feedback for status changes

---

## 🗣️ Live Feedback

For coded mock interactions, consider polite status announcements for:
- Save success
- Validation failure
- Filter result count where necessary
- Approval update
- Reassignment success

Avoid over-announcing routine changes.

---

## ✅ Review Checklist

- [ ] Status not color-only
- [ ] Contrast reviewed
- [ ] Keyboard primary flows tested
- [ ] Visible focus
- [ ] Tables semantically structured
- [ ] Forms labeled
- [ ] Errors associated
- [ ] Dialog focus managed
- [ ] Reduced motion supported
- [ ] Responsive zoom/reflow checked
