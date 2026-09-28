# FactoryDR — Methodology and Reproducibility Note

## Research structure

1. Define the narrow question: evidence applicability for a designated backup manufacturing route as the product changes.
2. Separate the technical-mechanism test from commercial validation.
3. Freeze Prototype 0 dataset, policy and candidate before held-out execution.
4. Keep evaluator outcomes sealed from the implementation context.
5. Compare held-out predictions only after execution.
6. Close Prototype 0 after the frozen experiment.
7. Conduct Phase 1D public-evidence shadow validation with explicit evidence grades and negative-evidence search.
8. Run an existing-system kill test against PLM, ERP, QMS, SCRM and adjacent change-intelligence platforms.
9. Make a build/park/kill decision rather than extending research indefinitely.

## Prototype 0 record

- Experiment: `FDR-P0-1.0`
- Candidate: `FDR-P0-CANDIDATE-1.0.0`
- Public dataset SHA-256: `d22f5771849b49ae50e3c9198325b98b620a0b30c586a423550f7aa0dbdf76bc`
- Held-out input SHA-256: `67997d8d841b4c5eba50dd6f528cf0c158aa93e2254478095c2e18df39eeacf4`
- Evaluator-private SHA-256: `7acf69d37f8ea9214c43145b1b8ad43b85dd49946ccdc092c05e78a6a75a2866`
- Candidate archive SHA-256: `293f361c2853dd2a21ac2806fa1bacfed1f441f7ef27b3638899c9876cbce76b`
- Frozen policy SHA-256: `b298df5ec8f0920b6e78f8024746d3744473542e7d6b9f52a8bbfd699ddb180c`
- Combined result: **20/20 scenario vectors; 240/240 CR classifications; 0 critical false READY.**

## Limitations

- Synthetic experiment only.
- No independent manufacturing-engineer review of the dependency graph/oracle.
- Same-author correlation remains a limitation.
- Public-evidence shadow validation is not customer discovery and cannot prove willingness to pay.
- Vendor documentation is capability evidence, not adoption/outcome proof.

## Final disposition

**PARK — SERVICES / INTERNAL TOOL / RESEARCH**
