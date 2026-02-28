---
id: "93717a42-e773-46a9-9485-3852cc5dfb98"
title: Migration Control Board
created: "2026-02-28T09:43:24.568Z"
updated: "2026-02-28T09:44:17.639Z"
type: board
---
# Board

## Settings
- viewMode: board
- gridSnap: 20
- listSort: placement
- backgroundColor: #f8fafc
- backgroundPattern: grid
- backgroundImage: 
- backgroundImageMode: fill
- zonePreset: kanban
- contrastMode: auto
- contrastLevel: normal

## Items
- {"id":"pm-checklist","kind":"note","ref":"Work/Projects/Platform Migration/API Migration Checklist.md","title":"API Migration Checklist","expanded":true,"x":24,"y":132,"w":300,"h":230}
- {"id":"pm-iam","kind":"text","ref":"","title":"Dependency: IAM policy approval from Security","color":"#fde68a","tags":["dependency"],"x":36,"y":390,"w":286,"h":120}
- {"id":"pm-service-arch","kind":"note","ref":"Work/Projects/Platform Migration/Service Architecture.md","title":"Service Architecture","x":380,"y":132,"w":300,"h":190}
- {"id":"pm-risk-sync","kind":"text","ref":"","title":"Escalation: data sync lag in staging","color":"#fecaca","tags":["risk","ops"],"x":392,"y":346,"w":282,"h":122}
- {"id":"pm-aks-review","kind":"note","ref":"Work/Meetings/AKS Architecture Review.md","title":"AKS Architecture Review","x":740,"y":132,"w":300,"h":190}
- {"id":"pm-adr","kind":"note","ref":"Work/Projects/Platform Migration/Architecture Decision Record.md","title":"Architecture Decision Record","x":1098,"y":132,"w":312,"h":190}
- {"id":"pm-tasks","kind":"note","ref":"My Tasks.md","title":"My Tasks","rolledUp":true,"opacity":0.92,"x":1108,"y":352,"w":300,"h":110}
- {"id":"pm-win","kind":"text","ref":"","title":"Cutover rehearsal completed with zero rollback events","color":"#bbf7d0","tags":["evidence"],"locked":true,"x":1106,"y":506,"w":300,"h":122}

## Drawings
- {"id":"pm-title","kind":"text","x":20,"y":18,"w":560,"h":64,"text":"Platform Migration Control Board","fontSize":28,"fontFamily":"Inter","fontWeight":"700","textAlign":"left","layer":40}
- {"id":"pm-arrow-flow","kind":"arrow","x":0,"y":0,"points":[330,220,380,220,430,220],"stroke":"#2563eb","strokeWidth":3,"lineStyle":"dashed","layer":15}
- {"id":"pm-highlight","kind":"rect","x":364,"y":100,"w":328,"h":430,"stroke":"#93c5fd","fill":"rgba(147,197,253,0.12)","strokeWidth":2,"lineStyle":"dashed","opacity":0.85,"layer":-1}
- {"id":"pm-signoff","kind":"text","x":1114,"y":470,"w":286,"h":40,"text":"Ready for sign-off","fontSize":16,"fontStyle":"italic","textDecoration":"underline","textAlign":"right","layer":35}

## Zones
- {"id":"pm-zone-backlog","title":"Backlog","x":0,"y":84,"w":340,"h":722,"color":"rgba(125,211,252,0.16)","layer":-5}
- {"id":"pm-zone-progress","title":"In Progress","x":352,"y":84,"w":340,"h":722,"color":"rgba(216,180,254,0.16)","layer":-5}
- {"id":"pm-zone-review","title":"Review","x":704,"y":84,"w":340,"h":722,"color":"rgba(125,211,252,0.16)","layer":-5}
- {"id":"pm-zone-done","title":"Done","x":1056,"y":84,"w":360,"h":722,"color":"rgba(187,247,208,0.16)","layer":-5}

