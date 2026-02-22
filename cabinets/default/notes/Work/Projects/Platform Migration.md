---
id: "a18e93af-80ed-484d-8396-7905155669bf"
title: Platform Migration
created: "2026-02-22T11:07:01.014Z"
updated: "2026-02-22T11:13:21.499Z"
type: project
---
## Platform Migration to Azure Kubernetes

Migration of our core analytics platform from on-premise VMs to Azure Kubernetes Service (AKS). This is the highest priority initiative for Q1 2026.

### Vision

Move all 12 microservices from legacy VM deployment to containerized AKS infrastructure, achieving auto-scaling, improved observability, and 40% reduction in hosting costs.

### Milestones

- [x] Infrastructure planning and AKS cluster provisioning <!-- task:pm-1 -->
- [x] Container images for all services <!-- task:pm-2 -->
- [x] CI/CD pipeline with GitHub Actions <!-- task:pm-3 -->
- [ ] Migrate staging environment (3 services) @Erik <!-- task:pm-4 -->
- [ ] Load testing on staging due:2026-03-01 <!-- task:pm-5 -->
- [ ] Migrate production - batch 1 (auth, gateway, users) due:2026-03-15 @Alex <!-- task:pm-6 -->
- [ ] Migrate production - batch 2 (analytics, reporting, ETL) due:2026-04-01 @Maja <!-- task:pm-7 -->
- [ ] Migrate production - batch 3 (remaining services) due:2026-04-15 <!-- task:pm-8 -->
- [ ] Decommission old VMs due:2026-05-01 <!-- task:pm-9 -->

### Technical Notes

**AKS Cluster Configuration:**
- Region: Norway East
- Node pools: System (3x Standard_D4s_v3) + User (auto-scale 2-8x Standard_D8s_v3)
- Ingress: NGINX with cert-manager for TLS
- Monitoring: Prometheus + Grafana stack

**Key Decisions:**
1. Using Helm charts for all deployments
2. Azure Container Registry for image storage
3. Managed PostgreSQL stays as-is (not moving to containers)
4. Redis cluster deployed in AKS alongside services

### Risks

| Risk | Impact | Mitigation |
|------|--------|------------|
| Service downtime during migration | High | Blue-green deployment strategy |
| Data sync issues | Medium | Parallel run for 2 weeks per batch |
| Team capacity | Medium | Dedicated migration sprint for each batch |

### Links

- [AKS Documentation](https://learn.microsoft.com/en-us/azure/aks/)
- [[Work/Meetings/Platform Migration Kickoff|Kickoff Meeting Notes]]
- [[Work/Meetings/AKS Architecture Review|Architecture Review]]