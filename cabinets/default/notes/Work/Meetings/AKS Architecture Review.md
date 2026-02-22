---
id: "17356fe9-cec2-43c7-9be6-b4430ab13f7e"
title: AKS Architecture Review
created: "2026-02-22T11:11:59.174Z"
updated: "2026-02-22T11:12:00.788Z"
type: meeting
---
## AKS Architecture Review\n\n**Date:** 2026-02-05\n**Attendees:** Alex Lindström, Erik Hansen, Maja Solberg, Jonas Berg, Lisa Park (Security)\n**Location:** Virtual (Teams)\n\n### Discussion\n\nErik walked through the proposed cluster architecture. Two node pools: system (always-on, 3 nodes) and user (auto-scaling 2-8 nodes).\n\nLisa raised security points:\n- Azure Policy for pod security (no privileged containers)\n- Network policies to isolate namespaces\n- Key Vault integration for secrets\n- Regular vulnerability scanning\n\n**Monitoring decision:** Prometheus + Grafana in-cluster, with Azure Monitor as backup.\n\n### Architecture\n\n\n\n### Action Items\n\n- [x] Erik: Implement network policies <!-- task:ar-1 -->\n- [x] Jonas: Set up Key Vault CSI driver <!-- task:ar-3 -->\n- [ ] Alex: Configure Grafana dashboards due:2026-02-20 @Alex <!-- task:ar-4 -->