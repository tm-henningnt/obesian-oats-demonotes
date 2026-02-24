---
type: graph
title: "Security Requirements"
---
# Security Requirements

## Mermaid
```mermaid
%% preset: requirement
requirementDiagram

    requirement auth_req {
    id: SEC001
    text: Users must authenticate via OAuth
    risk: high
    verifymethod: test
    }

    requirement encrypt_req {
    id: SEC002
    text: Personal config must be AES256 encrypted
    risk: high
    verifymethod: inspection
    }

    requirement token_req {
    id: SEC003
    text: Tokens stored in IndexedDB only
    risk: medium
    verifymethod: analysis
    }

    requirement byok_req {
    id: SEC004
    text: AI keys never leave the browser
    risk: high
    verifymethod: test
    }

    element github_oauth {
    type: module
    docRef: platform/github/client.ts
    }

    element crypto_module {
    type: module
    docRef: platform/crypto.ts
    }

    github_oauth - satisfies -> auth_req
    crypto_module - satisfies -> encrypt_req
    token_req - deriveReqt -> auth_req
    byok_req - refines -> encrypt_req
```
