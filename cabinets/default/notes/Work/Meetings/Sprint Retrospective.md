---
id: "943b8af4-68cd-48ea-9f41-03efe2d277ea"
title: Sprint 14 Retrospective
created: "2026-02-22T11:12:02.154Z"
updated: "2026-02-22T11:14:15.500Z"
type: meeting
---
# Sprint 14 Retrospective

**Date:** 2026-02-14
**Attendees:** Alex Lindström, Erik Hansen, Maja Solberg, Sofie Dahl, Jonas Berg

## Agenda

1. What went well
2. What could be improved
3. Action items for next sprint

## Discussion

**What Went Well 🎉**
- Customer Dashboard SSO integration shipped ahead of schedule
- Platform migration staging environment is up and running
- Team morale is high, good energy in daily standups
- Zero production incidents this sprint!

**What Could Be Improved 🔧**
- Too many context switches between migration and dashboard work
- Code review turnaround time averaging 2 days — target is < 1 day
- Flaky integration tests blocking PRs
- Documentation falling behind

## Decisions

- Implement code review rotation to reduce turnaround time
- Dedicate 30 min/week per person for documentation
- Fix flaky tests before adding new ones

## Action Items

- [ ] Alex: Create review rotation schedule due:2026-02-20 @Alex <!-- task:2wvp07a4 -->
- [ ] Jonas: Fix flaky Selenium tests due:2026-02-21 @Jonas <!-- task:ey6f46mb -->
- [ ] Everyone: 30 min/week for documentation <!-- task:gi378huq -->
