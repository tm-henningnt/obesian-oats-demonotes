---
id: "36b073d5-fa55-40e7-bc16-964ba5f3cf21"
title: Scratch Pad
created: "2026-02-22T11:15:23.384Z"
updated: "2026-02-22T11:15:25.429Z"
---
## Scratch Pad

### AKS migration command cheat sheet

```bash
# Get cluster credentials
az aks get-credentials --resource-group rg-northwind-prod --name aks-northwind

# Check pods
kubectl get pods -n production

# View logs
kubectl logs -f deployment/api-gateway -n production

# Scale deployment
kubectl scale deployment analytics-service --replicas=3 -n production

# Port forward for debugging
kubectl port-forward svc/grafana 3000:3000 -n monitoring
```

### SQL query for dashboard performance testing

```sql
SELECT 
  customer_id,
  DATE_TRUNC('day', created_at) as day,
  COUNT(*) as events,
  AVG(response_time_ms) as avg_response
FROM analytics_events 
WHERE created_at >= NOW() - INTERVAL '30 days'
GROUP BY customer_id, day
ORDER BY day DESC;
```

### Conference talk CFP notes

Title idea: "From VMs to Kubernetes: A Practical Migration Story"
Conference: NDC Oslo (June 2026)
CFP deadline: March 15
Format: 45-minute talk
Abstract: TODO — write this weekend

### Random links to check later

- https://roadmap.sh/devops — DevOps roadmap (share with Jonas?)
- https://learnk8s.io — Good K8s learning resources
- Checked out Warp terminal — interesting AI features but sticking with iTerm2 for now