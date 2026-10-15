# Standalone repository split

Moved the trading-dashboard subtree history to its own repository. Preserved
all five source files byte-for-byte before adding standalone build profiles,
artifact budgeting, provenance and CI. Existing old source is retained for
consumers still pinned to crypto-tools. No host authentication/pause policy,
service deployment or domain API changes are part of this move.

Stable all-target compiler, strict Clippy and Rust1.85all-target checks pass.
Existing renderer tests were retained with history and were not executed.
License remains UNLICENSED; the owner selected MIT only for market-data.

Consumers should use this repository's exact reviewed commit, then check their
working tree independently before adopting it. Do not overwrite the existing
Polydoghound changes or infer a paper/live release from a dependency move.
