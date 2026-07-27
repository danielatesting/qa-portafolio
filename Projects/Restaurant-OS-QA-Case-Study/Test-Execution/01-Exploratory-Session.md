# Exploratory Testing Session 01

## Session Information

| Property | Value |
|----------|-------|
| Session ID | ETS-001 |
| Tester | Daniela Gutierrez |
| Date | 2026-07-26 |
| Module | Dashboard & Reservation Workflow |
| Duration | 60 minutes |
| Testing Type | Exploratory Testing |
| Status | Completed |

---

# Mission

Explore the Dashboard and Reservation workflow to understand how the application supports daily restaurant operations, identify potential risks, and document observations for future testing.

---

# Areas Explored

## Dashboard

- Overview Cards
- Quick Actions
- Operations Overview
- Content Overview
- Marketing Health
- System Health
- Attention Needed
- Navigation Controls

## Reservation Workflow

- Create Reservation
- Pending Reservations
- Edit Reservation
- Move Reservation
- Cancel Reservation
- Seat Guest
- Complete Reservation

---

# Test Workflow

The following workflow was executed during the session:

Dashboard

↓

Create Reservation

↓

Edit Reservation

↓

Move Reservation

↓

Cancel Reservation

↓

Seat Guest

↓

Complete Reservation

↓

Review Dashboard statistics

---

# Observations

## Reservation Creation

**Result:** PASS

A new reservation was successfully created from the Dashboard.

No issues were encountered during the creation process.

---

## Reservation Management

**Result:** PASS

Successfully performed:

- Edit reservation
- Cancel reservation
- Review reservation details

Basic reservation management behaved as expected.

---

## Move Reservation

**Result:** Needs Investigation

The "Move Reservation" dialog allowed selecting another table, but no obvious confirmation or save action was visible.

It was unclear whether the reservation was successfully reassigned.

### Recommendation

Verify the expected business behavior with the product team before classifying this as a defect.

---

## Seat Guest

**Result:** Observation

The reservation could be marked as "Seated."

No obvious method to undo this action was found.

Further investigation is required to determine whether this is intentional.

---

## Complete Reservation

**Result:** Needs Investigation

The system allowed a reservation scheduled for a future date to be marked as completed.

This may represent a business logic issue, depending on the intended workflow.

---

## Dashboard Widgets

Dashboard widgets loaded successfully.

Marketing statistics and reservation information updated after reservation actions.

Further validation is required to determine whether all dashboard metrics reflect business rules correctly.

---

# Risks Identified

- Reservation status transitions may allow unexpected state changes.
- Reservation movement workflow may lack clear user feedback.
- Dashboard statistics require validation against expected business rules.

---

# Questions Raised

- Should future reservations be allowed to be completed?
- How should the Move Reservation workflow confirm changes?
- Should seated reservations support an undo action?
- What business rules determine Dashboard statistics?

---

# Bugs Found

No confirmed defects were reported during this session.

Several observations require clarification before being classified as bugs.

---

# New Test Scenarios Identified

- Validate reservation status transitions.
- Verify Move Reservation workflow.
- Verify reservation completion rules.
- Validate Dashboard widget updates.
- Verify reservation statistics consistency.

---

# Lessons Learned

The Dashboard provides quick access to the restaurant's operational workflows.

Exploring complete business workflows revealed more valuable observations than testing individual buttons in isolation.

Several potential issues require clarification of business rules before they can be reported as defects.

---

# Follow-up Actions

- Explore Guest Management (CRM).
- Validate reservation business rules.
- Continue documenting Dashboard behavior.
- Create formal bug reports for confirmed issues.

---

# Document Information

| Property | Value |
|----------|-------|
| Author | Daniela Gutierrez |
| Version | 1.1 |
| Status | Completed |
