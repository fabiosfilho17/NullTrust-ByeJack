# NullTrust-ByeJack

## 1) What it is
A practical Zero Trust lab focused on **Entra ID + Conditional Access + (optional) Intune Compliance** and a **Python script** that audits posture via **Microsoft Graph** and generates a report.

## 2) Why it exists (objective)
- To consolidate real fundamentals of identity and access (Zero Trust) with justified decisions.
- To build an “architecture + security + automation” portfolio (not just UI).
- To create an applied study path for AZ-305/AZ-500 while progressing through the courses.

## 3) Scope (what's included / what's excluded)
### Included now
- Entra ID: fictitious users, groups, basic roles, break-glass accounts.
- Conditional Access: 5 demonstrable policies with documented exceptions.
- Evidence: prints/outputs + decision notes.

- Automation (Python): collect CA policies and privileged principals via Graph and generate Markdown reports.

### Out for now
- SIEM/SOC (Sentinel), advanced detections/alerts.

- Penetration testing, network scanning, scanners, extensive infrastructure hardening.

- Any new feature before closing a phase with a deliverable.

## 4) Deliverables (what becomes a portfolio)
- `README.md`: scope, phases, decisions, and readiness criteria.

- `docs/decisions.md`: short record of decisions (why / impact / trade-off).

- `docs/threat-model.md`: simple threat model (what I protect, from whom, how).

- `src/`: Python script for generating reports.

- `evidence/`: evidence per phase (screenshots with masked data when necessary).

## 5) Roadmap (phases)
- **Phase 0 — Governance:** closed scope + repo structure + doc templates.

- **Phase 1 — Identities:** users/groups (admin bootstrap, 2 break-glass, Finance/IT/Contractor profiles) + MFA.

- **Phase 2 — Conditional Access:** 5 policies + validation and evidence.

- **Phase 3 — Intune Compliance (optional):** compliance profiles + compliant vs. non-compliant test.

- **Phase 4 — Python Report:** Graph script → Markdown report (CA + privileged principals).

## 6) Doneness criteria per phase
A phase is only “completed” when:
- there is evidence in `evidence/`,
- there is at least 1 decision recorded in `docs/decisions.md`,

- and the README/roadmap has been updated if anything has changed.

## 7) Security Warnings
- Never commit secrets/tokens.
- Use fictitious data whenever possible.

- Evidence should mask sensitive information.
