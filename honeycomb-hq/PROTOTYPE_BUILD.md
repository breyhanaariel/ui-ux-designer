# 💻 Honeycomb HQ — Coded Prototype Implementation

## 🌼 Status

✅ A **front-end-only interactive prototype** is implemented in `site/index.html`. It behaves like a credible SaaS product without pretending to have production infrastructure.

The code should support the portfolio case study by proving:
- Responsive implementation
- Stateful interactions
- Complex UI composition
- Accessibility
- Design-system thinking
- Realistic edge states

---

## 🛠 Implemented Stack

- Semantic HTML
- Responsive CSS
- Vanilla JavaScript
- Local in-memory mock data

The dependency-free implementation keeps the portfolio demo fast, portable, and easy to deploy.

---

## 📁 Repository Structure

```
honeycomb-hq/
├── README.md
├── UX_CASE_STUDY.md
├── PRODUCT_REQUIREMENTS.md
├── FLOWS_AND_IA.md
├── INTERACTION_SPEC.md
├── ACCESSIBILITY.md
├── PROTOTYPE_BUILD.md
└── assets/

site/
└── index.html  # portfolio + all three working interactive showcases

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

## ✅ Implemented Prototype Areas

- Responsive application shell
- Dashboard attention queue
- Projects data table
- Search and filtering
- Project detail interaction
- Create-project flow
- Approval and invoice state interactions
- Responsive table-to-card transformation
- Empty states
- Modal focus handling
- Reduced-motion support
- Keyboard interaction

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

`vercel.json` is committed at the repository root and routes all portfolio paths to the static application. A real public URL will be added only after the Vercel account connection authorizes publication.
