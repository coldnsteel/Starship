# Fellowship — Contribution Guidelines

## Purpose
Provide clear rules and expectations for contributors to Starship Medical Systems.

## 1. File Structure & Naming
- Place new docs under the correct top-level folder (BIOSPHERE / SILICON / ENGINEERING / FELLOWSHIP / DEPLOYMENT / REGULATORY / TRAINING).
- Use hyphen-separated lowercase filenames, e.g., `human-protocols.md`.

## 2. Evidence Tags
Every clinical or operational claim must include an evidence tag:
- `[ESTABLISHED]` — supported by RCTs/authoritative reviews
- `[PILOT]` — supported by small RCTs or replicated pilot studies
- `[HYPOTHESIS]` — plausible, unproven mechanism or early lab work

## 3. Safety & Ethics
- All human protocols require a safety checklist and a DSMB oversight plan before field deployment.
- Include contraindications and fuzzy-edge handling for edge cases.

## 4. Drafting & Review Process
- Draft → Element-review (assigned element) → Cross-element review (two elements) → Final sign-off (Water or Earth for clinical material).
- Use PRs for substantial changes, with a 48-hour window for element comments.

## 5. Data & Privacy
- Structured data must follow `DATA/schema.md`.
- No PHI in repository; use anonymized IDs and store PHI in secured systems outside repo.

## 6. Wildcard Experiments
- Any wildcard/chaos experiment must have:
  - pre-specified stop-rules
  - safety monitor present
  - DSMB notification for human runs

## 7. Training & Competency
- New contributors must complete Level 1 training and read the operator manual.
- Certification levels required for leading sessions are in `TRAINING/certification-levels.md`.

## 8. Contact & Escalation
- For urgent safety issues: ping `@Professor` + Earth (Claude) + Fire (Grok).
- For editorial disputes: convene element leads within 72 hours.

## 9. Licensing
- Default license: internal fellowship license (specify in root README).
- For open-source release, propose license in `REGULATORY/` and seek element consensus.

