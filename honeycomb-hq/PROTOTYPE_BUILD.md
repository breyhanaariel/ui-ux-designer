# 💻 Honeycomb HQ — Coded Prototype Plan

## 🌼 Goal

Build a **front-end-only interactive prototype** that behaves like a credible SaaS product without pretending to have production infrastructure.

The code should support the portfolio case study by proving:
- Responsive implementation
- Stateful interactions
- Complex UI composition
- Accessibility
- Design-system thinking
- Realistic edge states

---

## 🛠 Planned Stack

- React
- TypeScript
- Tailwind CSS
- React Router
- Lightweight local state
- Static/mock JSON data

Optional only if useful:
- Recharts for a small number of meaningful visualizations
- Lucide icons
- Testing Library
- Vitest

Avoid adding libraries solely to make the stack look larger.

---

## 📁 Planned Prototype Structure

```
honeycomb-hq/
├── README.md
├── UX_CASE_STUDY.md
├── PRODUCT_REQUIREMENTS.md
├── FLOWS_AND_IA.md
├── INTERACTION_SPEC.md
├── ACCESSIBILITY.md
├── PROTOTYPE_BUILD.md
├── assets/
│   └── README.md
└── prototype/
    ├── package.json
    ├── src/
    │   ├── app/
    │   ├── components/
    │   ├── features/
    │   ├── data/
    │   ├── hooks/
    │   ├── types/
    │   └── utils/
    └── ...
```

The `prototype/` application should only be added once real implementation begins.

---

## 🧩 Feature Modules

Suggested code organization:
- `dashboard`
- `projects`
- `clients`
- `approvals`
- `team`
- `billing`
- `activity`

Shared components:
- AppShell
- Sidebar
- MobileNav
- DataTable
- FilterBar
- StatusBadge
- HealthBadge
- Dialog
- FormField
- EmptyState
- ErrorState
- Skeleton
- Toast

---

## 🗃️ Mock Data

Create realistic but fictional:
- 12–20 projects
- 8–12 clients
- 6–10 team members
- Deliverables/approvals
- Invoices
- Recent activity

Include edge cases:
- Overdue
- No owner
- At risk
- Awaiting client
- Empty result
- Long names
- Disabled user
- Late invoice

Do not use real client data.

---

## ✅ Interactive Prototype Milestones

### Milestone 1 — Shell
- Responsive navigation
- Routes
- Layout
- Mock data

### Milestone 2 — Dashboard
- Attention queue
- Deadlines
- Approvals
- Billing warning
- Workload signal

### Milestone 3 — Projects
- Table
- Search
- Sort
- Filters
- Project detail

### Milestone 4 — Actions
- Create project
- Update status
- Approval action
- Reassignment
- Invoice follow-up state

### Milestone 5 — Quality
- Empty/loading/error states
- Keyboard review
- Reduced motion
- Mobile
- Basic component tests

---

## ♿ Implementation Requirements

Use semantic HTML before ARIA.

Required:
- Buttons for actions, not clickable divs
- Labels for form controls
- Table markup for true tabular data
- `aria-sort` where appropriate
- Dialog semantics/focus management
- Visible focus
- `prefers-reduced-motion`
- Status announcements only where useful

---

## 🌷 Deployment

Prepare `prototype/` so it can deploy independently to a static host such as Vercel or Netlify.

Do not add a fake deployment URL to the portfolio. Add the link only after a real deployment exists.
