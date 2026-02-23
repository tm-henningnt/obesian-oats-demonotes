---
id: "ea23caaa-111e-4af8-a7e6-73b6aac6fe48"
title: Customer Feedback Session
created: "2026-02-22T11:25:54.387Z"
updated: "2026-02-22T11:25:57.444Z"
type: meeting
---
# Customer Feedback Session — Acme Corp

**Date:** 2026-02-12
**Attendees:** Alex Lindström, Sofie Dahl, Henrik Voss (Acme Corp, VP Analytics), Anna Berge (Acme Corp, Data Analyst)
**Location:** Virtual (Teams)

## Agenda

Demo our dashboard prototype and gather feedback from pilot customer.

## Discussion

Henrik was impressed with the overall look and feel. Called it "much better than what we have now with the PDF reports." Anna had more detailed feedback:

**Positive:**
- Loved the drag-and-drop widget layout
- Date range picker with presets is exactly what they need
- Loading speed was good (1.8s on staging)
- Dark mode option was a nice surprise

**Concerns:**
- Need ability to compare current period vs. previous period (YoY, MoM)
- Table widget needs column sorting and search
- Export to Excel must preserve number formatting (not just raw CSV)
- Want email alerts when metrics exceed thresholds (not just scheduled reports)

**Feature Requests:**
1. Comparison periods (high priority)
2. Dashboard commenting/annotations
3. Embeddable widgets via iframe (for their internal portal)
4. Custom color themes beyond just dark/light

## Action Items

- [ ] Sofie: Add comparison period toggle to chart widgets due:2026-03-05 @Sofie <!-- task:n7bsh55p -->
- [ ] Erik: Implement column sort/search in table widget due:2026-03-01 @Erik <!-- task:1xqm2je6 -->
- [ ] Alex: Evaluate email alerting feasibility for v1.1 due:2026-02-25 @Alex <!-- task:fs8ph3u9 -->
- [ ] Sofie: Mockup embeddable widget concept due:2026-03-10 @Sofie <!-- task:m9zdkd61 -->

## Decisions

> "If you ship this by April, we can cancel our Tableau license." — Henrik Voss

> "The fact that I can drag widgets around and save my own layout is game-changing for us." — Anna Berge
