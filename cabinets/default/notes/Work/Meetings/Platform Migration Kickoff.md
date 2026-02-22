---
id: "24cb36b3-acce-4b68-aef0-f3e83220bb99"
title: Platform Migration Kickoff
created: "2026-02-22T11:11:56.344Z"
updated: "2026-02-22T11:11:57.873Z"
type: meeting
---
## Platform Migration Kickoff\n\n**Date:** 2026-01-15\n**Attendees:** Alex Lindström, Erik Hansen, Maja Solberg, Jonas Berg, Karin Olsen (CTO)\n**Location:** Conference Room North\n\n### Agenda\n\n1. Project overview and timeline\n2. Resource allocation\n3. Risk assessment\n\n### Discussion\n\nKarin opened with the business case: our current VM costs are €18k/month and growing. AKS target is €10k/month with better scaling. Board has approved the migration budget.\n\nErik presented the technical assessment. All 12 services are already containerized for local dev, but production Dockerfiles need hardening. Estimated 2-3 days per service.\n\nMaja raised concerns about the ETL pipeline — it currently uses local file system for staging data. Need to move to Azure Blob Storage. **Decision:** Use Azure Blob with SAS tokens.\n\n### Action Items\n\n- [x] Alex: Set up AKS cluster in dev subscription <!-- task:mk-2 -->\n- [x] Jonas: Draft CI/CD pipeline design document <!-- task:mk-3 -->\n- [x] Alex: Schedule weekly migration sync <!-- task:mk-5 -->\n\n### Key Decisions\n\n1. ✅ Use Azure Blob Storage for ETL staging\n2. ✅ Helm charts for all deployments\n3. ✅ Blue-green deployment strategy for zero-downtime