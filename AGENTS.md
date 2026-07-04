# AGENTS.md

Version: 1.0
Status: Approved
Owner: MoneyPulse Leadership

## Purpose

This file defines how automated development work must be performed on MoneyPulse.

## Required Reading Order

Before implementing anything, read:

1. `docs/00_GOVERNANCE/PRODUCT_MANIFESTO.md`
2. `docs/00_GOVERNANCE/PRINCIPLES.md`
3. `docs/01_PRODUCT/PRODUCT.md`
4. `docs/03_ENGINEERING/ARCHITECTURE.md`
5. `docs/04_AI/DECISION_ENGINE.md`
6. `docs/05_MANAGEMENT/TASKS.md`

## Non-Negotiable Rules

- Never invent undocumented features.
- Never add complexity without a documented reason.
- Documentation wins over code when conflicts exist.
- Keep the Decision Engine deterministic and explainable.
- Language models may explain results, but may not calculate financial decisions.
- Mobile-first always.
- TypeScript strict mode always.
- Backend must expose simple REST APIs.
- Update `CHANGELOG.md` after every completed task.

## Product Rule

Every screen must help the user answer one of these questions:

- How much can I safely spend today?
- Can I afford this before I buy it?
- What happens next?
- What should I improve?

## Engineering Rule

The core must be pure:

- no database access;
- no HTTP calls;
- no hidden state;
- same input, same output.

## Commit Discipline

Every commit should be small, focused and explain what changed.
