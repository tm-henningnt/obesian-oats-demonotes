---
id: "org-chart-001"
title: Team Org Chart
created: "2026-02-23T13:50:00.000Z"
updated: "2026-02-23T16:06:11.166Z"
type: graph
---
# Team Org Chart

## Mode
- orgchart

## Mermaid
```mermaid
%% mode: orgchart
flowchart TB
  CTO["Karin Olsen\nCTO"]
  ALEX["Alex Lindström\nTech Lead"]
  JONAS["Jonas Berg\nEngineering Manager"]
  ERIK["Erik Hansen\nBackend Developer"]
  MAJA["Maja Solberg\nDevOps Engineer"]
  LISA["Lisa Park\nSecurity Engineer"]
  SOFIE["Sofie Dahl\nFrontend Lead"]
  OMAR["Omar Patel\nQA Engineer"]
  NINA["Nina Strand\nUX Designer"]
  step_10["Step 10"]
  CTO --> ALEX
  CTO --> JONAS
  ALEX --> ERIK
  ALEX --> MAJA
  ALEX --> LISA
  JONAS --> SOFIE
  JONAS --> OMAR
  JONAS --> NINA
  JONAS --> step_10
```
