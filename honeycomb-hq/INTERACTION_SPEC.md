# ✨ Honeycomb HQ — Interaction Specification

## 🌼 Interaction Principles

- Favor visible system status.
- Keep high-frequency actions close to the object they affect.
- Make destructive/financial actions explicit.
- Use optimistic updates only where reversal is safe.
- Preserve context when opening details from dense lists.
- Never rely on hover for essential information.

---

## 📊 Tables

### Row behavior
- Entire row may open detail if interactive affordance is clear.
- Row-level menu remains separately keyboard accessible.
- Selected/hover states must not be color-only.

### Sorting
- One clear active sort state.
- Direction visible in text/icon and available to assistive tech.

### Filters
- Active filters visible after menu closes.
- Show count where useful.
- “Clear all” available for multiple filters.
- Empty filtered state explains why no data appears.

### Responsive
At smaller widths:
- Remove lower-priority columns.
- Promote important metadata into stacked row/card content.
- Avoid shrinking text excessively.

---

## 🔎 Search

- Clear search input label.
- Debounce UI may be simulated in code.
- Loading feedback for delayed mock results.
- “No results” differs from “data failed to load.”

---

## 🚦 Health & Status

Project **status** and **health** are separate.

Example:
> Active · At Risk

Use icon/text or label/text combinations so meaning survives without color.

Tooltip may explain calculated mock health but must not contain essential-only information.

---

## 📝 Forms

- Persistent labels.
- Required fields marked consistently.
- Inline error near field.
- Summary for multi-error complex form where useful.
- Preserve entered values after failure.
- Disable submit only when reason is obvious; otherwise validate after action.

---

## 🗑️ Destructive Actions

Examples:
- Archive project
- Remove member
- Delete draft

Require confirmation when impact is meaningful.

Confirmation should name the affected item:
> Archive “Moonlight Rebrand”?

Avoid generic “Are you sure?”

---

## 💰 Billing Actions

Mock billing state changes should:
- State the current invoice status.
- State the resulting status.
- Avoid pretending a real payment was processed.
- Record mock activity in the prototype.

---

## ✅ Approval Actions

Approval detail should show:
- Deliverable
- Version
- Client
- Requested date
- Due date
- Decision state
- Related project

On decision:
- Clear success feedback
- Project context updates
- Undo only if the model supports safe reversal

---

## 🔔 Notifications

Prioritize meaningful changes:
- Mention / assignment
- Approval decision
- Deadline risk
- Client response
- Invoice state

Allow read/unread state.

Avoid notification spam in mock data.

---

## ⌨️ Keyboard & Focus

- Sidebar navigation keyboard accessible
- Menus open/close predictably
- Dialog focus trapped and restored
- Escape closes overlays where appropriate
- Visible focus ring
- Focus does not disappear after dynamic updates

---

## 🎞️ Motion

Use for:
- Drawer/dialog transition
- State change confirmation
- Reordering feedback

Avoid:
- Decorative continuous motion
- Large parallax
- Motion-only status indication

Provide reduced-motion CSS behavior in the coded prototype.
