---
id: "b71b5dfc-4998-445d-93a6-25d4af4d75a3"
title: API Migration Checklist
created: "2026-02-22T11:25:39.864Z"
updated: "2026-02-23T18:36:40.209Z"
type: todo
---
# API Migration Checklist

<!-- oats:todo-settings {"viewMode":"list","listLayout":"area","boardGrouping":"priority"} -->

## High Priority
- [x] Auth Service — containerized, health checks added [cat:Batch 1 — Auth & Gateway] <!-- task:8tatrug4 -->
- [x] API Gateway — containerized, rate limiting configured [cat:Batch 1 — Auth & Gateway] <!-- task:c0fnk0u0 -->
- [x] User Service — containerized, DB connection pooling updated [cat:Batch 1 — Auth & Gateway] <!-- task:dqcymq3g -->
- [ ] Staging deployment for batch 1 @Jonas @2026-03-01 [cat:Batch 1 — Auth & Gateway] <!-- task:nleybk9o -->
- [ ] Load testing batch 1 @Erik @2026-03-10 [cat:Batch 1 — Auth & Gateway] <!-- task:0oawlbs0 -->
- [ ] Production cutover batch 1 @Alex @2026-03-15 [cat:Batch 1 — Auth & Gateway] <!-- task:2oo76n0h -->

## Normal
- [x] Analytics Service — containerized [cat:Batch 2 — Core Analytics] <!-- task:gtjs88bl -->
- [ ] Reporting Service — needs refactoring for stateless operation @Erik [cat:Batch 2 — Core Analytics] <!-- task:hx78s23g -->
- [ ] ETL Pipeline — Blob Storage migration in progress @Maja [cat:Batch 2 — Core Analytics] <!-- task:ambpvgfg -->
- [ ] Staging deployment for batch 2 @2026-03-20 [cat:Batch 2 — Core Analytics] <!-- task:5lpg3j3i -->
- [ ] Production cutover batch 2 @2026-04-01 [cat:Batch 2 — Core Analytics] <!-- task:au3f95ua -->

## Low Priority
- [ ] Notification Service — needs webhook URL updates [cat:Batch 3 — Remaining] <!-- task:5acohfq6 -->
- [ ] Search Service — Elasticsearch sidecar needed [cat:Batch 3 — Remaining] <!-- task:ni9kiqay -->
- [ ] Scheduler Service — cron job conversion to K8s CronJob [cat:Batch 3 — Remaining] <!-- task:2grvpmlz -->
- [ ] File Service — storage driver change required [cat:Batch 3 — Remaining] <!-- task:ckmkf41q -->
- [ ] Config Service — replace with ConfigMaps @Jonas [cat:Batch 3 — Remaining] <!-- task:mdrlvkqu -->
- [ ] Audit Log Service — high write volume, test scaling @Erik [cat:Batch 3 — Remaining] <!-- task:4ebahjb3 -->
