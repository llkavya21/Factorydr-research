# Implementation limitations — FDR-P0-CANDIDATE-1.0.0

1. The engine implements only the frozen `FDR-P0-1.0` structured-data semantics.
2. It does not inspect CAD, firmware binaries, physical equipment, supplier operations, quality systems or real manufacturing execution.
3. The dependency graph and evidence facts are authored synthetic inputs; correct implementation cannot prove those facts correspond to real engineering conditions.
4. Some frozen reason-code labels are broader than ideal for edge cases; these interpretation points were documented before held-out execution rather than tuned from held-out outcomes.
5. No held-out packet, held-out expected state or held-out case description was available or processed during candidate freeze.
