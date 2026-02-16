============================================================================
# Project Decisions
============================================================================

## [2026-02-16] Decision: Scope closed by phases
- Context: avoid infinite scope and the project becoming a "mini-SOC".
- Decision: only ID + CA + (optional) Intune + Python report are included.
- Trade-off: fewer features now, more consistency and delivery.
- Rejected alternatives: include Sentinel/detections from the beginning.

## [2026-02-16] Decision: Evidence as part of "done"
- Context: without evidence, it seems like progress has been made, but it proves nothing.
- Decision: every phase requires evidence/ + documented decision.
- Trade-off: more documentation work, much more portfolio value.

- ## [2026-02-16] Decision: Break-glass accounts
- Context: Conditional Access misconfiguration can lock administrators out; this lab must remain recoverable.
- Decision: Create 2 break-glass accounts excluded from all Conditional Access policies and without MFA/CA dependency.
- Trade-off: Higher risk if credentials are compromised.
- Mitigations: Very long unique passwords, strict storage (offline/password manager), no daily use, and any login is treated as an incident and documented.

## [2026-02-16] Decision: Name Account Patterns
- Context: Name standards to use on the accounts and groups
- Decision: Will use short, simple and known names to be closer to a true narrative. 
- Trade-off: avoid creating too much to not get lost on the scripts creation.
- Mitigations: Use known names to be easier to remeber, will be more realistic in the screenshots
- Naming pattern is in <i>/docs/naming-standard.md

