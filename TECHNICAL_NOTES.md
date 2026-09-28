# Technical notes

## State model

Each continuity requirement resolves to one of:

`CURRENT · STALE · REVIEW_REQUIRED · MISSING · BLOCKED · UNKNOWN`

Overall readiness is derived deterministically:

- `MISSING` or `BLOCKED` → `NOT_READY`
- `UNKNOWN` → `UNKNOWN`
- `STALE` or `REVIEW_REQUIRED` → `REVALIDATION_REQUIRED`
- all `CURRENT` → `READY_WITHIN_SCOPE`

`READY_WITHIN_SCOPE` means the bounded synthetic evidence model passes. It does **not** mean a physical factory is production-ready.

## Frozen experiment identifiers

- Experiment: `FDR-P0-1.0`
- Candidate: `FDR-P0-CANDIDATE-1.0.0`
- Candidate archive SHA-256: `293f361c2853dd2a21ac2806fa1bacfed1f441f7ef27b3638899c9876cbce76b`
- Frozen policy SHA-256: `b298df5ec8f0920b6e78f8024746d3744473542e7d6b9f52a8bbfd699ddb180c`
- Public dataset SHA-256: `d22f5771849b49ae50e3c9198325b98b620a0b30c586a423550f7aa0dbdf76bc`

## Architecture

```text
structured product + manufacturing state
                │
                ▼
        dependency relationships
                │
                ▼
        CR01–CR12 deterministic rules
                │
                ▼
 CURRENT / STALE / REVIEW_REQUIRED /
 MISSING / BLOCKED / UNKNOWN
                │
                ▼
 READY_WITHIN_SCOPE / REVALIDATION_REQUIRED /
 NOT_READY / UNKNOWN
```

## Reproducibility discipline

The candidate and policy were frozen before held-out inputs were released. Held-out expected states and evaluator material were not available to the implementation context during execution.

The complete frozen public dataset, source code, tests and exact hash manifests are preserved in the private master research archive. This public GitHub repository is intentionally curated for portfolio readability rather than publishing answer-bearing/private experiment material.

## Deliberate technical exclusions

The engine does not inspect CAD geometry, firmware binaries, physical equipment, supplier operations, real quality systems, manufacturing execution, capacity, tacit knowledge or onsite conditions.
