---
id: "b71b5dfc-4998-445d-93a6-25d4af4d75a3"
title: API Migration Checklist
created: "2026-02-22T11:25:39.864Z"
updated: "2026-02-22T11:25:43.326Z"
type: todo
---
# API Migration Checklist

<!-- oats:todo-settings {"listLayout":"area"} -->

Track the migration status of each microservice API from VM to AKS.

## High Priority

- [x] Auth Service — containerized, health checks added [cat:Batch 1 — Auth & Gateway] <!-- task:api-1 -->
- [x] API Gateway — containerized, rate limiting configured [cat:Batch 1 — Auth & Gateway] <!-- task:api-2 -->
- [x] User Service — containerized, DB connection pooling updated [cat:Batch 1 — Auth & Gateway] <!-- task:api-3 -->
- [ ] Staging deployment for batch 1 due:2026-03-01 @Jonas [cat:Batch 1 — Auth & Gateway] <!-- task:api-4 -->
- [ ] Load testing batch 1 due:2026-03-10 @Erik [cat:Batch 1 — Auth & Gateway] <!-- task:api-5 -->
- [ ] Production cutover batch 1 due:2026-03-15 @Alex [cat:Batch 1 — Auth & Gateway] <!-- task:api-6 -->

## Normal

- [x] Analytics Service — containerized [cat:Batch 2 — Core Analytics] <!-- task:api-7 -->
- [ ] Reporting Service — needs refactoring for stateless operation @Erik [cat:Batch 2 — Core Analytics] <!-- task:api-8 -->
- [ ] ETL Pipeline — Blob Storage migration in progress @Maja [cat:Batch 2 — Core Analytics] <!-- task:api-9 -->
- [ ] Staging deployment for batch 2 due:2026-03-20 [cat:Batch 2 — Core Analytics] <!-- task:api-10 -->
- [ ] Production cutover batch 2 due:2026-04-01 [cat:Batch 2 — Core Analytics] <!-- task:api-11 -->

## Low Priority

- [ ] Notification Service — needs webhook URL updates [cat:Batch 3 — Remaining] <!-- task:api-12 -->
- [ ] Search Service — Elasticsearch sidecar needed [cat:Batch 3 — Remaining] <!-- task:api-13 -->
- [ ] Scheduler Service — cron job conversion to K8s CronJob [cat:Batch 3 — Remaining] <!-- task:api-14 -->
- [ ] File Service — storage driver change required [cat:Batch 3 — Remaining] <!-- task:api-15 -->
- [ ] Config Service — replace with ConfigMaps @Jonas [cat:Batch 3 — Remaining] <!-- task:api-16 -->
- [ ] Audit Log Service — high write volume, test scaling @Erik [cat:Batch 3 — Remaining] <!-- task:api-17 -->

See [[Work/Projects/Platform Migration|Project overview]] for milestones.
