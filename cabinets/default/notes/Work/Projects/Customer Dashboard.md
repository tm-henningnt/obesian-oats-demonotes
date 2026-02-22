---
id: "02b1c66e-2063-404d-913c-09b8fc30e112"
title: Customer Dashboard
created: "2026-02-22T11:11:53.656Z"
updated: "2026-02-22T11:12:24.077Z"
type: project
---
## Customer-Facing Analytics Dashboard

Self-service analytics dashboard for enterprise customers. Replaces the current static PDF reports with interactive, real-time visualizations.

### Vision

Give customers direct access to their data through a modern, responsive dashboard with customizable widgets, scheduled reports, and API access.

### Milestones

- [x] User research and wireframes <!-- task:cd-1 -->
- [x] Design system and component library <!-- task:cd-2 -->
- [x] Authentication with customer SSO <!-- task:cd-3 -->
- [x] Core dashboard layout with drag-and-drop widgets <!-- task:cd-4 -->
- [ ] Chart library integration (bar, line, pie, map) due:2026-02-28 @Sofie <!-- task:cd-5 -->
- [ ] Data API with row-level security due:2026-03-10 @Erik <!-- task:cd-6 -->
- [ ] Scheduled report generation (PDF export) due:2026-03-20 <!-- task:cd-7 -->
- [ ] Beta launch with 3 pilot customers due:2026-04-01 <!-- task:cd-8 -->

### Tech Stack

- **Frontend:** React 19, Recharts, TanStack Table
- **Backend:** Node.js, Fastify, PostgreSQL
- **Auth:** Azure AD B2C with custom policies
- **Hosting:** Vercel (frontend) + Azure Container Apps (API)

### Customer Requirements

1. **Real-time data** — refreshed every 5 minutes minimum
2. **Custom date ranges** — flexible filtering
3. **Export to Excel** — critical for finance teams
4. **White-labeling** — customers want their own branding
5. **Mobile responsive** — executives check dashboards on phones