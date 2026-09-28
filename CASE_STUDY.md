# FactoryDR — 2-minute case study

## Research question

Can deterministic software determine when product or manufacturing changes make previously valid evidence for a designated backup manufacturing route no longer demonstrably applicable to the current product configuration?

## Why this question mattered

Manufacturing continuity evidence can involve BOMs, approved sources, firmware, tooling, process instructions, test systems, qualifications and recovery-drill records. A backup site can have been qualified previously while later product/configuration changes make part of that evidence stale, missing, blocked or uncertain.

## What I built

A bounded deterministic evidence-applicability mechanism using:

- 12 continuity requirements (`CR01`–`CR12`);
- structured evidence and revision state;
- a dependency graph;
- deterministic requirement-state precedence;
- canonical JSON outputs and SHA-256 commitments;
- frozen candidate code before held-out execution.

The engine uses structured facts and deterministic rules.

## Technical result

| Measure | Result |
|---|---:|
| Development scenario vectors | 16 / 16 exact |
| Development requirement states | 192 / 192 exact |
| Held-out overall outcomes | 4 / 4 exact |
| Held-out requirement states | 48 / 48 exact |
| Combined scenario vectors | 20 / 20 |
| Combined requirement classifications | 240 / 240 |
| Critical false `READY_WITHIN_SCOPE` | 0 |

**Technical disposition:** `BOUNDED DETERMINISTIC MECHANISM SURVIVED`

This result is limited to the frozen synthetic experiment.

## Commercial falsification

I then separated the commercial question from the technical result and reviewed public evidence across OEM/contract-manufacturing practices plus PLM, ERP, QMS and supply-chain-risk platforms.

The evidence supported that configuration/readiness drift and recurring continuity work are real. However, modern PLM/ERP/QMS/SCRM systems can represent or automate substantial portions of the workflow, and public evidence did not establish a separately budgeted buyer for the residual FactoryDR layer.

**Commercial disposition:** `PARK — SERVICES / INTERNAL TOOL / RESEARCH`

## Why this project matters as portfolio evidence

It demonstrates:

- technical/product hypothesis design;
- deterministic systems thinking;
- experiment freezing and reproducibility;
- held-out evaluation discipline;
- primary-source commercial research;
- build-vs-buy and incumbent substitution analysis;
- willingness to park a technically successful idea when the company thesis is not sufficiently supported.

See [CLAIM_BOUNDARIES.md](CLAIM_BOUNDARIES.md) before using results outside this repository.
