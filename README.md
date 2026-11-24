# AI-Powered Financial Reconciliation & Investigation Platform

A planned B2C full-stack platform for analyzing financial activity across multiple accounts, reconciling transactions, investigating potential anomalies, and exploring financial scenarios with evidence-grounded AI assistance.

> **Status:** Planning / initial setup. Features listed below are goals, not implemented capabilities.

## Planned MVP

- Import user-provided CSV and OFX financial statements, with a one-click synthetic demo.
- Normalize transactions from multiple accounts into a consistent data model.
- Match internal transfers and credit-card payments without double-counting.
- Detect potential duplicates and recurring-charge changes for user review.
- Explore cash-flow scenarios through interactive visualizations.
- Use a restricted AI investigation assistant to explain findings using verified records.

### Planned technology stack

| Layer | Technology |
| --- | --- |
| Frontend | Next.js, React, TypeScript, Tailwind CSS |
| Backend | Python, FastAPI, Pydantic |
| Database | PostgreSQL, SQLAlchemy |
| Analytics | Pandas or Polars; graph matching and anomaly detection |
| AI | Gemini / OpenAI, optional LangGraph tool orchestration |
| Testing | Pytest, Hypothesis, Playwright |
| Delivery | Docker, GitHub Actions, cloud deployment |

## Engineering principles

- Financial calculations use exact decimal or integer-cent arithmetic; never binary floating-point for money.
- Deterministic calculations, not LLM outputs, establish financial results.
- Missing evidence and uncertain transaction matches are explicitly visible.
- Users review findings before taking any financial action.
- Prioritize local or synthetic demonstration data before handling sensitive personal statements.

## Development plan

1. Model transactions, accounts, and the reconciliation invariants.
2. Implement CSV/OFX ingestion and Python/FastAPI endpoints.
3. Build cross-account transfer matching and anomaly checks.
4. Create the Next.js dashboard and interactive transaction views.
5. Add a constrained, read-only AI investigation workflow.
6. Add tests, security checks, observability, and deploy a public demo.

See [docs/PROJECT_SCOPE.md](docs/PROJECT_SCOPE.md) for the initial MVP boundaries.

## Disclaimer

This is an engineering project in development, not a bank or a source of personalized financial advice. Do not upload real confidential statements until the security and privacy design is implemented and evaluated.
