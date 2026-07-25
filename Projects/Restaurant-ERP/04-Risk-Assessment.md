# Risk Assessment

## Purpose

This document identifies the application's highest-risk areas based on business impact. It is used to prioritize exploratory testing and guide future test planning.

---

## Risk Rating

| Risk | Description |
|-------|-------------|
| 🔴 Critical | Failure prevents core restaurant operations. |
| 🟠 High | Major functionality is affected but work can continue with limitations. |
| 🟡 Medium | Feature is important but does not stop daily operations. |
| 🟢 Low | Cosmetic or secondary functionality. |

---

# Module Risk Assessment

| Module | Business Impact | Risk | Priority |
|----------|----------------|------|----------|
| Front of House | Restaurant operations, reservations, seating | 🔴 Critical | P1 |
| System | Application configuration, permissions, settings | 🔴 Critical | P1 |
| Dashboard | Operational overview and shortcuts | 🟠 High | P2 |
| Workforce | Employee management | 🟠 High | P2 |
| Content | Menus, blog posts, events | 🟡 Medium | P3 |
| Marketing | Newsletters and campaigns | 🟡 Medium | P3 |
| Inbox | Notifications and messages | 🟢 Low | P4 |

---

# Initial Testing Order

1. Dashboard
2. Front of House
3. System
4. Workforce
5. Content
6. Marketing
7. Inbox

---

## Notes

This assessment is based on the current understanding of the application and will be updated as new modules and workflows are explored.
