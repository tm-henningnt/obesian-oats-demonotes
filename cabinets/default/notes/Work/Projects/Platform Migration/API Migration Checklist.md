---
id: "b71b5dfc-4998-445d-93a6-25d4af4d75a3"
title: API Migration Checklist
created: "2026-02-22T11:25:39.864Z"
updated: "2026-02-22T11:25:43.326Z"
type: todo
---
## API Migration Checklist

Track the migration status of each microservice API from VM to AKS.

### Batch 1 — Auth & Gateway (Target: March 15)

- [x] Auth Service — containerized, health checks added <!-- task:api-1 -->
- [x] API Gateway — containerized, rate limiting configured <!-- task:api-2 -->
- [x] User Service — containerized, DB connection pooling updated <!-- task:api-3 -->
- [ ] Staging deployment for batch 1 due:2026-03-01 @Jonas <!-- task:api-4 -->
- [ ] Load testing batch 1 due:2026-03-10 @Erik <!-- task:api-5 -->
- [ ] Production cutover batch 1 due:2026-03-15 @Alex <!-- task:api-6 -->

### Batch 2 — Core Analytics (Target: April 1)

- [x] Analytics Service — containerized <!-- task:api-7 -->
- [ ] Reporting Service — needs refactoring for stateless operation @Erik <!-- task:api-8 -->
- [ ] ETL Pipeline — Blob Storage migration in progress @Maja <!-- task:api-9 -->
- [ ] Staging deployment for batch 2 due:2026-03-20 <!-- task:api-10 -->
- [ ] Production cutover batch 2 due:2026-04-01 <!-- task:api-11 -->

### Batch 3 — Remaining Services (Target: April 15)

- [ ] Notification Service — needs webhook URL updates <!-- task:api-12 -->
- [ ] Search Service — Elasticsearch sidecar needed <!-- task:api-13 -->
- [ ] Scheduler Service — cron job conversion to K8s CronJob <!-- task:api-14 -->
- [ ] File Service — storage driver change required <!-- task:api-15 -->
- [ ] Config Service — replace with ConfigMaps @Jonas <!-- task:api-16 -->
- [ ] Audit Log Service — high write volume, test scaling @Erik <!-- task:api-17 -->

### Pre-Migration Checks (Per Service)

- [ ] Dockerfile reviewed and hardened
- [ ] Health check endpoint (/healthz) implemented
- [ ] Graceful shutdown handling
- [ ] Resource limits defined (CPU/memory)
- [ ] Helm chart created and tested
- [ ] Secrets migrated to Key Vault
- [ ] Monitoring dashboards configured
- [ ] Runbook updated

See [[Work/Projects/Platform Migration|Project overview]] for milestones.