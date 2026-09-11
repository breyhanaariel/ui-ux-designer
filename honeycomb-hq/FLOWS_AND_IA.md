# 🗺️ Honeycomb HQ — Flows & Information Architecture

## 🌼 Navigation Model

### Primary
1. Overview
2. Projects
3. Clients
4. Approvals
5. Team
6. Billing
7. Activity
8. Settings

### Global
- Search
- Create
- Notifications
- Workspace switcher
- Profile

---

## 🐝 Desktop App Shell

```
┌──────────────────────────────────────────────────┐
│ Workspace / Global Search / Create / Alerts / Me │
├────────────┬─────────────────────────────────────┤
│ Overview   │                                     │
│ Projects   │            Page Content             │
│ Clients    │                                     │
│ Approvals  │                                     │
│ Team       │                                     │
│ Billing    │                                     │
│ Activity   │                                     │
│ Settings   │                                     │
└────────────┴─────────────────────────────────────┘
```

---

## 📱 Mobile App Shell

Prioritize frequent actions.

Suggested bottom navigation:
- Home
- Projects
- Approvals
- More

Global create can remain as a contextual action rather than occupying permanent navigation.

---

## 🌻 Flow 1 — Triage Today's Work

```
Open Overview
  ↓
Scan Needs Attention
  ↓
Choose at-risk project
  ↓
Read risk reason + next action
  ↓
Open blocker / approval / task
  ↓
Take action
  ↓
Return to updated priority queue
```

Design question:
Can the user understand **why** an item is prioritized without opening several screens?

---

## ✅ Flow 2 — Resolve Client Approval

```
Approvals
  ↓
Filter = Client action required
  ↓
Open deliverable
  ↓
Review version + context
  ↓
Send reminder OR record response
  ↓
Approval status changes
  ↓
Project activity / health updates
```

Edge cases:
- Approval already resolved in another state
- Deliverable replaced
- Client contact unavailable
- Deadline has passed

---

## 🧩 Flow 3 — Create Project

```
Create
  ↓
Project
  ↓
Choose client
  ↓
Basics
  ↓
Dates / milestones
  ↓
Team
  ↓
Review
  ↓
Create
```

Prefer a short multi-step experience over one giant form if testing supports it.

Preserve entered data on validation errors.

---

## 👥 Flow 4 — Rebalance Workload

```
Team
  ↓
Capacity warning
  ↓
Person detail
  ↓
Review upcoming assigned work
  ↓
Select task
  ↓
Reassign
  ↓
Confirm
  ↓
Capacity state updates
```

Do not use red/yellow/green alone to communicate capacity.

---

## 💰 Flow 5 — Overdue Invoice

```
Billing
  ↓
Filter = Overdue
  ↓
Invoice detail
  ↓
Review client/project context
  ↓
Record follow-up / status
  ↓
Activity entry
```

Financial actions should have explicit status language and safe confirmations.

---

## 🔎 Search

Global search may return:
- Projects
- Clients
- People
- Deliverables
- Invoices

Results should group by type rather than flattening unrelated entities.

---

## 🌷 Empty States

Design distinct empty states for:
- No projects yet
- No search results
- No filtered results
- No pending approvals
- No urgent work
- No overdue invoices

“No urgent work” should feel positive but still provide useful next navigation.

---

## ⚠️ Error / Failure States

Include:
- Failed page data
- Failed action
- Validation error
- Stale state / conflict
- Permission denied
- Offline / reconnecting

Each error should explain:
1. What happened
2. Whether data was saved
3. What the user can do next
