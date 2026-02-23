---
id: "6f089fd1-ea1d-4ed6-a839-314c9393168e"
title: Conference Talk Ideas
created: "2026-02-22T11:26:12.156Z"
updated: "2026-02-23T15:44:29.603Z"
---
## Conference Talk Ideas

### NDC Oslo 2026 (CFP deadline: March 15)

**Primary idea:** "From VMs to Kubernetes: A Practical Migration Story"

- 45-minute talk
- Real-world lessons from migrating 12 microservices to AKS
- Cover: planning, Helm charts, CI/CD, monitoring, rollback strategies
- Include war stories and things that went wrong
- Target audience: Backend developers and DevOps engineers

**Outline draft:**

1. Why we migrated (costs, scaling, developer experience)
2. Planning phase — what we wish we knew
3. Containerization gotchas (stateful services, local file deps)
4. CI/CD pipeline design with GitHub Actions
5. The migration itself — blue-green deployment in practice
6. Monitoring and observability (Prometheus + Grafana)
7. Lessons learned and metrics (before/after comparison)
8. Q&A

### JavaZone 2026 (September)

**Idea:** "Building Multi-Tenant Analytics Dashboards with React and Row-Level Security"

- Focus on the Customer Dashboard project
- How to implement row-level security that actually works
- Performance optimization for real-time data visualization
- White-labeling patterns

### Lightning Talk Ideas (10 min)

- "ADRs: The Documentation Your Future Self Will Thank You For"
- "5 kubectl Commands That Will Save Your Production"
- "Why I Switched to Markdown for Everything"

### Speaking Tips (from last year's NDC)

- Practice 3x minimum with timer
- Have a backup laptop with slides on USB
- Arrive 30 min early to test projector
- Bring water bottle and throat lozenges
- End 5 min early for Q&A — never run over

```mermaid
%% oats-graph-ref: {"version":1,"id":"graphref-9vclxw5h","storeId":"bd7da143-c242-4a57-858f-5d64292f2705","cabinetId":"default","path":"cabinets/default/notes/Quick Notes/Conference Talk Ideas Mindmap.md","title":"Conference Talk Ideas Mindmap","sha":"172cb439873c370044ab220583c17f87c2c3bd2a","importedAt":"2026-02-23T15:44:26.590Z","updatedAt":"2026-02-23T15:44:26.590Z"}
%% mode: mindmap
flowchart TB
  ROOT("Conference Talks") --> NDC("NDC Oslo 2026")
  ROOT --> JZ("JavaZone 2026")
  ROOT --> LIGHT("Lightning Talks")
  NDC --> NDC1("VMs to Kubernetes")
  NDC1 --> NDC1A("Planning lessons")
  NDC1 --> NDC1B("Helm charts")
  NDC1 --> NDC1C("CI/CD pipeline")
  NDC1 --> NDC1D("War stories")
  NDC --> NDC2("Monitoring story")
  NDC2 --> NDC2A("Prometheus + Grafana")
  NDC2 --> NDC2B("Alert fatigue")
  JZ --> JZ1("Multi-tenant dashboards")
  JZ1 --> JZ1A("Row-level security")
  JZ1 --> JZ1B("React performance")
  JZ1 --> JZ1C("White-labeling")
  LIGHT --> L1("ADRs for future self")
  LIGHT --> L2("kubectl lifesavers")
  LIGHT --> L3("Markdown for everything")
```
