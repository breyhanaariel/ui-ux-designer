# 🍯 Honeycomb HQ — UX Case Study

> **Status:** Case-study framework complete. Research, visual artifacts, and prototype evidence will be added as they are created.

---

## 1. 🌼 Overview

Honeycomb HQ is a responsive agency-operations SaaS concept for small creative teams.

The project is designed to test my ability to solve a more complex product problem than a consumer mobile experience: multiple roles, dense information, cross-project risk, approvals, deadlines, workload, and billing.

### Core design question
> **How might an agency operator identify and act on the work that needs attention today without checking several disconnected tools?**

---

## 2. 🐝 Context & Problem Space

A small creative agency may manage:
- 10–50 active clients
- Multiple projects per client
- Internal and external deadlines
- Client approvals
- Team assignments
- Files and deliverables
- Project communication
- Invoices and payment status

The challenge is not simply storing this information.

The challenge is **helping the user know what matters now**.

---

## 3. 🎯 Working Hypotheses

These are hypotheses to validate, not findings.

1. Agency operators lose time switching between tools to reconstruct project status.
2. Existing project dashboards often prioritize counts/charts over actionable risk.
3. Approvals become bottlenecks when they are buried inside individual projects.
4. Workload risk is easier to prevent when upcoming deadlines and assignments are visible together.
5. A role-aware dashboard can reduce noise by showing each user the actions relevant to them.

---

## 4. 🔎 Research Plan

### Questions
- How do small agencies currently track client work?
- What triggers an operator to check project status?
- Which conditions make a project feel “at risk”?
- How are approvals requested and followed up?
- How is team workload estimated?
- Where do invoices intersect with project decisions?
- What information is useful on mobile?

### Planned methods
- Competitive audit
- 5–8 semi-structured interviews
- Workflow mapping
- Task prioritization exercise
- Prototype usability testing

📌 Visual slot: `assets/01-research-synthesis.png`

---

## 5. 👥 Provisional Roles

Use roles rather than fictional demographic personas until research supports more detail.

### Agency Owner / Operations Lead
Needs an overview of risk, revenue, deadlines, and team capacity.

### Project Manager
Needs to coordinate tasks, dependencies, approvals, and client communication.

### Account Lead
Needs client context, deliverable status, next actions, and approval history.

### Contributor
Needs a focused view of assigned work, due dates, files, and comments.

After research, revise these roles based on actual workflow patterns.

📌 Visual slot: `assets/02-role-needs.png`

---

## 6. 🗺️ Information Architecture

Primary navigation:

```
Overview
Projects
Clients
Approvals
Team
Billing
Activity
Settings
```

Global utilities:
- Search
- Create
- Notifications
- Help
- Profile / workspace switcher

📌 Visual slot: `assets/03-information-architecture.png`

---

## 7. 🌻 Primary Flows

### Flow A — Resolve a project risk
`Dashboard → At-risk item → Project detail → Identify blocker → Take action → Status updates`

### Flow B — Client approval
`Approvals queue → Deliverable → Review context → Send / remind / record decision → Project updates`

### Flow C — Create a project
`Projects → New Project → Client → Scope / dates → Team → Milestones → Confirm`

### Flow D — Rebalance workload
`Team → Capacity warning → Team member → Upcoming work → Reassign → Confirm`

### Flow E — Follow up on overdue invoice
`Billing → Overdue → Invoice detail → Contact / mark status → Activity recorded`

📌 Visual slot: `assets/04-core-user-flows.png`

---

## 8. ✏️ Wireframe Exploration

The first wireframe phase should focus on hierarchy, not branding.

### Dashboard explorations
Compare at least three models:
1. Metric-led dashboard
2. Activity-led dashboard
3. Attention / risk-led dashboard

Document why the final approach was selected.

### Required low-fidelity screens
- Dashboard
- Projects list
- Project detail
- Approvals queue
- Team workload
- Billing
- Mobile priority view

📌 Visual slot: `assets/05-wireframe-exploration.png`

---

## 9. 📊 Dashboard Decision Framework

Every dashboard module should answer at least one question:

- Does this require action?
- Is something at risk?
- Did something important change?
- Is there a deadline?
- Is there a financial consequence?
- Who owns the next step?

If a card only looks impressive but does not help answer one of these, question whether it belongs.

---

## 10. 🧩 Tables, Filters & Data Density

The projects surface should demonstrate professional table design.

### Recommended columns
- Project
- Client
- Health
- Status
- Owner
- Next milestone
- Due date
- Budget / billing signal
- Updated

### Filters
- Health
- Status
- Client
- Owner
- Date range
- Approval state

### UX requirements
- Persistent active-filter feedback
- Clear reset
- Sort indicator
- Search
- Empty filtered state
- Keyboard-operable controls
- Mobile transformation strategy

📌 Visual slot: `assets/06-projects-table.png`

---

## 11. 🎨 Visual Design

The visual system should be professional with a recognizable warm brand.

### Foundations
- Honey/amber accent
- Slate neutral scale
- Semantic success/warning/error/info colors
- Clear typography hierarchy
- 4/8-based spacing scale
- Moderate radii
- Subtle surface elevation
- Strong focus treatment

📌 Visual slot: `assets/07-visual-foundations.png`

---

## 12. ✨ High-Fidelity Screens

Minimum showcase set:
1. Dashboard
2. Projects table
3. Project detail
4. Approvals queue
5. Team workload
6. Billing / invoice detail
7. Create-project flow
8. Mobile overview
9. Mobile project detail
10. Error / empty / loading states

📌 Visual slot: `assets/08-final-ui-overview.png`

---

## 13. 🧪 Usability Testing

### Suggested sample
5–8 people familiar with managing projects, clients, teams, or similar operational workflows.

### Tasks
- Find the project most in need of attention.
- Identify what is blocking it.
- Find deliverables waiting for client approval.
- Filter projects owned by a specific person.
- Reassign an upcoming task.
- Find an overdue invoice.
- Create a new project.

### Record
- Completion
- Incorrect paths
- Hesitation
- Misread statuses
- Filter mistakes
- Assistance needed
- Qualitative comments

Do not convert a tiny qualitative sample into inflated percentages.

📌 Visual slot: `assets/09-usability-findings.png`

---

## 14. ♿ Accessibility Review

Review:
- Keyboard navigation
- Focus visibility
- Table semantics
- Form labels
- Validation errors
- Status meaning beyond color
- Dialog focus management
- Target sizes
- Contrast
- Responsive zoom / reflow
- Reduced motion

📌 Visual slot: `assets/10-accessibility-review.png`

---

## 15. 💻 Prototype & Handoff

The coded prototype should demonstrate that design decisions can survive implementation.

Include:
- Component inventory
- Responsive states
- Interaction rules
- Validation behavior
- Loading/empty/error states
- Accessibility notes
- Mock-data schema

📌 Visual slot: `assets/11-handoff-and-code.png`

---

## 16. 🌷 Reflection

When the project is complete, document:
- What assumptions research disproved
- Which dashboard model changed most
- How density was balanced with scannability
- Where mobile required workflow changes rather than simple stacking
- Which implementation constraint changed the design
- What would be measured after launch
