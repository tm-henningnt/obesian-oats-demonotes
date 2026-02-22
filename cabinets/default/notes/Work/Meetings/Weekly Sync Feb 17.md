---
id: "e9a4023e-e4da-4001-9f87-04b968d0b2d0"
title: Weekly Sync — Feb 17
created: "2026-02-22T11:12:30.884Z"
updated: "2026-02-22T11:14:17.350Z"
type: meeting
---
# Weekly Team Sync

**Date:** 2026-02-17
**Attendees:** Alex, Erik, Maja, Sofie, Jonas

## Agenda

1. Individual status updates
2. Blockers and dependencies
3. Decisions

## Discussion

- Alex: Working on Grafana dashboards for AKS monitoring. Meeting with Karin Thursday about Q2 roadmap.
- Erik: Finished network policy implementation. Starting on Customer Dashboard data API. Blocked on database schema review.
- Sofie: Chart library going well — bar and line charts done, working on pie charts. Will demo Wednesday.
- Maja: ETL Blob Storage migration is 80% complete. Found performance issue with large CSV imports.
- Jonas: Fixed 4 of 7 flaky tests. CI pipeline for AKS is green — deployed to staging yesterday.

## Decisions

- Chart annotations: Add to backlog for v1.1
- Alex will review DB schema by EOD Tuesday
- Team dinner: Friday Feb 21, 18:00 at Fiskeriet

## Action Items

- [ ] Alex: Review database schema by EOD Tuesday @Alex <!-- task:ws-1 -->
- [ ] Sofie: Demo chart library Wednesday @Sofie <!-- task:ws-2 -->
- [ ] Maja: Investigate CSV import performance issue @Maja <!-- task:ws-3 -->
