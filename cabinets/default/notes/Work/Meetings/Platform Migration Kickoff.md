---
id: "24cb36b3-acce-4b68-aef0-f3e83220bb99"
title: Platform Migration Kickoff
created: "2026-02-22T11:11:56.344Z"
updated: "2026-02-22T11:14:11.851Z"
type: meeting
---
## Platform Migration Kickoff

**Date:** 2026-01-15
**Attendees:** Alex Lindström, Erik Hansen, Maja Solberg, Jonas Berg, Karin Olsen (CTO)
**Location:** Conference Room North

### Agenda

1. Project overview and timeline
2. Resource allocation
3. Risk assessment

### Discussion

Karin opened with the business case: our current VM costs are €18k/month and growing. AKS target is €10k/month with better scaling. Board has approved the migration budget.

Erik presented the technical assessment. All 12 services are already containerized for local dev, but production Dockerfiles need hardening. Estimated 2-3 days per service.

Maja raised concerns about the ETL pipeline — it currently uses local file system for staging data. Need to move to Azure Blob Storage. **Decision:** Use Azure Blob with SAS tokens.

### Action Items

- [x] Alex: Set up AKS cluster in dev subscription <!-- task:mk-2 -->
- [x] Jonas: Draft CI/CD pipeline design document <!-- task:mk-3 -->
- [x] Alex: Schedule weekly migration sync <!-- task:mk-5 -->

### Key Decisions

1. ✅ Use Azure Blob Storage for ETL staging
2. ✅ Helm charts for all deployments
3. ✅ Blue-green deployment strategy for zero-downtime