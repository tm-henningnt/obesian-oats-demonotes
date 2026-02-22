---
id: "2f16037a-e508-4214-8f84-599582c33aca"
title: Team Agreements
created: "2026-02-22T11:26:03.448Z"
updated: "2026-02-22T11:26:06.596Z"
---
## Platform Team — Working Agreements

Last updated: February 2026. Reviewed quarterly.

### Communication

- **Daily standup:** 09:15, max 15 minutes, async option in #platform-standup for remote days
- **Slack response time:** Within 2 hours during work hours, no expectation outside 08-16
- **Deep work blocks:** Respect calendar blocks labeled "Focus Time" — no meetings or pings
- **Decisions:** Document in notes or Slack threads, not verbal-only

### Code Standards

- **PR reviews:** Must be reviewed within 1 business day
- **PR size:** Aim for < 400 lines changed. Split larger changes into stacked PRs
- **Tests required:** All PRs must include tests. Target 80% coverage per service
- **Branch naming:** `feature/JIRA-123-short-description` or `fix/JIRA-456-bug-name`
- **Commit messages:** Conventional commits (feat:, fix:, docs:, refactor:, test:)

### Meetings

- **No-meeting Wednesday afternoons** (13:00-17:00 protected for deep work)
- **Cameras on** for 1-on-1s and retros, optional for other meetings
- **Meeting notes** always taken and shared in Obesian Oats

### On-Call

- **Rotation:** Weekly, Monday to Monday
- **Response time:** 15 min for P1 (service down), 2 hours for P2
- **Escalation:** If not resolved in 30 min, escalate to team lead (Alex)
- **Compensation:** Day off in lieu for weekend incidents

### Definition of Done

- [ ] Code reviewed and approved
- [ ] Tests pass in CI (unit + integration)
- [ ] Documentation updated (API docs, runbook)
- [ ] Deployed to staging and smoke tested
- [ ] No known regressions
- [ ] Monitoring/alerting configured

### Team Values

1. **Trust over control** — We assume good intent and give autonomy
2. **Progress over perfection** — Ship iteratively, improve continuously
3. **Transparency** — Share context, decisions, and mistakes openly
4. **Sustainable pace** — No hero culture, no chronic overtime