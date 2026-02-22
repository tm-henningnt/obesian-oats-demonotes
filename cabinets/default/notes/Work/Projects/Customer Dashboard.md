---
id: "02b1c66e-2063-404d-913c-09b8fc30e112"
title: Customer Dashboard
created: "2026-02-22T11:11:53.656Z"
<<<<<<< LOCAL
updated: "2026-02-22T17:57:18.109Z"
=======
<<<<<<< LOCAL
updated: "2026-02-22T17:56:50.998Z"
=======
updated: "2026-02-22T17:01:11.939Z"
>>>>>>> REMOTE
>>>>>>> REMOTE
type: project
---
# Customer-Facing Analytics Dashboard

## Overview
Self-service analytics dashboard for enterprise customers. Replaces the current static PDF reports with interactive, real-time visualizations.

## Goals
1. Give customers direct access to their data through a modern, responsive dashboard
2. Customizable widgets and scheduled reports
3. API access for programmatic data retrieval

## Milestones
### Core Platform
- [x] User research and wireframes <!-- task:2wfpljp3 -->
- [x] Design system and component library <!-- task:jdnx00zw -->
- [x] Authentication with customer SSO <!-- task:o6kxfdo0 -->
- [x] Core dashboard layout with drag-and-drop widgets <!-- task:6pnofucg -->

### Beta Launch (2026-02-28 → 2026-04-01)
- [ ] Chart library integration (bar, line, pie, map) @Sofie @2026-02-28 <!-- task:97led2ji -->
- [ ] Data API with row-level security @Erik @2026-03-10 <!-- task:ntkqjym9 -->
- [ ] Scheduled report generation (PDF export) @2026-03-20 <!-- task:hv1kebgf -->
- [ ] Beta launch with 3 pilot customers @2026-04-01 <!-- task:9i379dpl -->

## Resources
- [React 19 Docs](https://react.dev) — Frontend framework
- [Recharts](https://recharts.org) — React charting library
- [TanStack Table](https://tanstack.com/table) — Table component

## Notes
- **Frontend:** React 19, Recharts, TanStack Table
- **Backend:** Node.js, Fastify, PostgreSQL
- **Auth:** Azure AD B2C with custom policies
- **Hosting:** Vercel (frontend) + Azure Container Apps (API)
- Real-time data refreshed every 5 minutes minimum
- Export to Excel must preserve number formatting
- White-labeling for customer branding
- Mobile responsive for executives
