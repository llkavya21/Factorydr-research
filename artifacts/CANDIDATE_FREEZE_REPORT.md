# Candidate freeze report — FDR-P0-CANDIDATE-1.0.0

- Experiment: `FDR-P0-1.0`
- Freeze date: `2026-09-24`
- Public dataset SHA-256: `d22f5771849b49ae50e3c9198325b98b620a0b30c586a423550f7aa0dbdf76bc`
- Machine policy SHA-256: `b298df5ec8f0920b6e78f8024746d3744473542e7d6b9f52a8bbfd699ddb180c`
- Baseline: `READY_WITHIN_SCOPE` with 12/12 `CURRENT`
- Development exact full-vector agreement: **16/16**
- Development CR agreement: **192/192**
- Expected-unaffected CR preservation: **160/160**
- Critical false READY: **0/4**
- Any oracle-nonready false READY: **0/13**
- Deterministic duplicate-run failures: **0**
- Reason/reference failures: **0 across 3628 checked reasons**
- Held-out inputs processed at freeze: **no**
- Held-out predictions generated at freeze: **no**

The candidate was frozen before held-out release. Any policy/source change after held-out release would have required a new candidate version.

**Claim boundary:** these results show reproduction of the frozen synthetic mechanism only.
