# Initial MVP scope

**Audience:** Individuals who want to investigate their own multi-account finances.

**Goal:** Build and deploy a robust Python-powered financial reconciliation platform with a polished web interface and meaningful agentic assistance.

## In scope

- Synthetic demo mode and opt-in CSV/OFX uploads.
- Account and transaction models, normalization, and import validation.
- Internal transfer matching with confidence scores and user confirmation.
- Explainable potential duplicate and recurring charge detections.
- Historical cash-flow views and bounded what-if scenarios.
- Read-only AI tools that retrieve evidence and run deterministic calculations.
- Login, isolation between users, automated tests, CI/CD, and deployed demo.

## Deferred until after MVP

- Direct connections to banks or money movement.
- Broad PDF/OCR format support and bounding-box evidence highlighting.
- Issuer-specific promotional credit-card interest and payment-allocation logic (PromoProof module).
- Investment or tax advice, autonomous financial decisions, and payment execution.

## Critical correctness checks

- No double-counting of verified transfers across accounts.
- Monetary calculations are exact for documented supported cases.
- Unresolved and ambiguous matches remain visible rather than silently merged.
- AI explanations cite source transactions and do not invent financial totals.

## First implementation task

Define the account/transaction schema, synthetic test fixture format, and transfer-matching test cases before building the dashboard.
