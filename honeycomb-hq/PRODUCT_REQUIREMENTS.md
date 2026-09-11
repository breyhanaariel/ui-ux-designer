# 📋 Honeycomb HQ — Product Requirements

## 🌼 Product Summary

Honeycomb HQ is a responsive operations workspace for small creative agencies.

### Product promise
**See what needs attention, understand why, and act without reconstructing project status across multiple tools.**

---

## 🐝 Target Team

Initial concept:
- 5–30-person creative agencies
- 10–50 active clients
- Project-based work
- Frequent client approvals
- Multiple simultaneous deadlines

These constraints are provisional until research is completed.

---

## 🎯 MVP Goals

The portfolio prototype should allow a user to:

1. Understand urgent work from the dashboard.
2. Browse/search/filter projects.
3. Inspect a project's current health and next action.
4. Review deliverables awaiting approval.
5. Understand basic team workload.
6. Identify overdue invoices.
7. Create or update a project.
8. Use the primary flows at desktop and mobile widths.

---

## 🚫 Non-Goals

For the portfolio MVP, do not attempt:
- Full accounting
- File storage backend
- Real email delivery
- Time tracking engine
- Real authentication
- Live multi-user collaboration
- Real payment processing
- AI automation

Use realistic mock states to design the workflows without pretending the product has production infrastructure.

---

## 🌻 Key Entities

### Workspace
Agency organization.

### User
Team member with role and permissions.

### Client
Organization/person receiving agency services.

### Project
Primary unit of work tied to a client.

### Milestone
Major project checkpoint.

### Task
Assignable work item.

### Deliverable
Artifact requiring review/approval.

### Approval
Decision state attached to a deliverable.

### Invoice
Billing record associated with client/project.

### Activity
Meaningful system event.

---

## 🌷 Project Health

Keep **status** and **health** distinct.

### Status
Lifecycle:
- Planned
- Active
- On Hold
- Complete
- Archived

### Health
Risk signal:
- On Track
- Needs Attention
- At Risk

Health may be informed by:
- Overdue milestone
- Blocked task
- Late approval
- Workload issue
- Approaching deadline

For the prototype, health logic may be deterministic mock logic and must be labeled as such.

---

## 💛 Dashboard Requirements

Dashboard should include:
- Priority / attention queue
- Upcoming deadlines
- Approval bottlenecks
- Team capacity warnings
- Overdue invoices
- Recent meaningful changes

Optional:
- Small summary metrics

Avoid making charts the primary information architecture.

---

## 🧩 Projects Requirements

Users can:
- Search
- Sort
- Filter
- Open project
- Create project
- Change supported project metadata

Show:
- Client
- Health
- Status
- Owner
- Due date / milestone
- Approval signal

---

## ✅ Approvals Requirements

Users can:
- View pending approvals
- See deliverable and project context
- Identify who must act
- Send/record reminder state in prototype
- Mark an approval outcome in mock interaction
- See resulting project-state change

---

## 👥 Team Requirements

Users can:
- View people and assigned workload
- Identify capacity warnings
- Open person detail
- Reassign mock work

The prototype should avoid pretending workload estimates are mathematically authoritative.

---

## 💰 Billing Requirements

Users can:
- Browse invoice states
- Find overdue invoices
- Open invoice detail
- Record a mock follow-up/status update

No payment processing is required.

---

## 📱 Responsive Requirements

### Desktop
All major workflows.

### Tablet
Preserve core filters/actions with selective column reduction.

### Mobile
Prioritize:
- Urgent work
- Project summary
- Approval action
- Notifications
- Quick update

Do not force desktop data tables into narrow horizontal scrolling unless justified.

---

## ♿ Quality Requirements

- Keyboard-operable primary flows
- Visible focus
- Semantic headings
- Proper form labels
- Error messaging
- Status not color-only
- Responsive reflow
- Reduced-motion support where motion is used

---

## 📈 Future Product Metrics

If this were a real product, consider:
- Time to identify highest-priority issue
- Approval turnaround time
- Project risk resolution time
- Number of overdue milestones
- User task success
- Repeated tool-switching / external status checks

These are product hypotheses, not portfolio results.
