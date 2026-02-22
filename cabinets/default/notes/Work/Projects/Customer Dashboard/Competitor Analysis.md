---
id: "8bcb335f-902a-4a19-9d98-663dfa06d948"
title: Competitor Analysis
created: "2026-02-22T11:25:49.581Z"
updated: "2026-02-22T11:25:52.735Z"
---
## Competitor Analysis — Analytics Dashboards

Analyzed 4 competing solutions to inform our dashboard design decisions.

### Feature Comparison

| Feature | Metabase | Looker | Tableau | PowerBI | **Ours** |
|---------|----------|--------|---------|---------|----------|
| Self-hosted option | ✅ | ❌ | ❌ | ❌ | ✅ |
| Custom branding | ❌ | ✅ | ✅ | ✅ | ✅ |
| Row-level security | ✅ | ✅ | ✅ | ✅ | ✅ |
| Scheduled reports | ✅ | ✅ | ✅ | ✅ | ✅ |
| Drag-drop layout | ❌ | ✅ | ✅ | ✅ | ✅ |
| API access | ✅ | ✅ | Limited | ✅ | ✅ |
| SSO (SAML/OIDC) | Enterprise | ✅ | ✅ | ✅ | ✅ |
| Mobile responsive | Partial | ✅ | ✅ | ✅ | ✅ |
| Price per user/mo | Free-$110 | $60+ | $70+ | $10+ | Custom |

### Key Takeaways

**Metabase** — Open source, great for internal use. Lacks the polish and white-labeling our customers need. No drag-and-drop dashboard editor.

**Looker (Google)** — Powerful modeling layer (LookML). But expensive and Google lock-in. Steep learning curve for end users.

**Tableau** — Industry standard for visual analytics. Too complex for our target users who want simple, pre-built dashboards. Overkill for our use case.

**PowerBI** — Best value at $10/user/month. Strong Excel integration. But difficult to white-label and embed for multi-tenant scenarios.

### Our Differentiation

1. **Built for multi-tenant SaaS** — row-level security and white-labeling from day one
2. **Simpler than Tableau/Looker** — pre-configured widgets, no query language needed
3. **API-first** — customers can build their own integrations
4. **Nordic data residency** — data stays in Norway/EU (important for our customers)
5. **Bundled with our analytics platform** — no additional data pipeline needed

### Pricing Strategy

Recommend per-tenant pricing (not per-user) to align with customer expectations:
- Starter: 3 dashboards, 10 users — bundled free
- Professional: Unlimited dashboards, 50 users — NOK 5,000/month
- Enterprise: Unlimited everything + API + SSO — NOK 15,000/month