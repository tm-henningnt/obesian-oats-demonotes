---
type: graph
title: "User Traffic Flow Sankey"
---
# User Traffic Flow Sankey

## Mermaid
```mermaid
%% preset: sankey
sankey-beta

Landing Page,Sign Up,350
Landing Page,Documentation,200
Landing Page,Demo,150
Landing Page,Bounce,300
Sign Up,GitHub Auth,280
Sign Up,Email Auth,70
GitHub Auth,Create Store,250
GitHub Auth,Drop Off,30
Email Auth,Create Store,50
Email Auth,Drop Off,20
Create Store,First Note,270
Create Store,Import Notes,30
First Note,Daily Active,200
First Note,Weekly Active,50
First Note,Churned,20
Import Notes,Daily Active,25
Import Notes,Weekly Active,5
Documentation,Sign Up,100
Documentation,Bounce,100
Demo,Sign Up,80
Demo,Bounce,70
```
