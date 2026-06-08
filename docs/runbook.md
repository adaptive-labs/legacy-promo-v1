---
category: runbook
title: Legacy Promo V1 runbook
description: On-call runbook for Legacy Promo V1.
related_entities:
  - legacy-promo-v1
related_teams:
  - checkout
---

# Legacy Promo V1 runbook

On-call guide for `legacy-promo-v1` (Checkout, tier low).

## Alerts

- **legacy-promo-v1-high-error-rate** — 5xx over 2% for 5m. Check upstream dependencies.
- **legacy-promo-v1-latency** — p99 over SLO. Check resource saturation.

## Common issues

- **Pod OOMKilled** — check memory limits and recent traffic spikes.
- **Crashloop** — check the last deploy and roll back if needed.

## Escalation

Page the Checkout on-call rotation.

