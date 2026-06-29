# Changelog

All notable changes to WAFBA are documented here. This project uses semantic
versioning adapted for an assessment instrument: MAJOR for changes that break
comparability with prior evaluations (added/removed/redefined domains or
markers), MINOR for additive changes that preserve comparability, PATCH for
wording, layout, and clarification.

## [1.0.0] — 2026-06-29

Initial public release.

### Instrument
- Sixteen-section assessment covering system identity, execution configuration,
  provenance confidence, task information, prompting strategy, eight functional
  behavioral rating domains, behavioral marker checklist, operator observations,
  evaluation conditions, overall functional impression, baseline consistency,
  and evaluator certification.
- Eight 1–5 functional rating domains with behavioral anchors.
- Behavioral marker checklist derived from documented real-world agent
  incidents.

### Repository
- Dual build: instrument specification (`docs/WAFBA-spec.md`) and working
  single-file form (`wafba.html`).
- CC BY-SA 4.0 license.
- Citation metadata (`CITATION.cff`).

### Known gaps (tracked for future versions)
- No structured antecedent / trigger capture (the "A" of the A-B-C
  contingency). Planned for a future revision.
- Several rating domains have a corresponding binary marker (e.g. Goal
  Maintenance / Goal Neglect); the two-tier graded-plus-threshold design is
  intentional but should be documented explicitly in-spec.
- No machine-readable (JSON) evaluation export. Planned, to support inter-rater
  reliability analysis across evaluators and sessions.
- No formal validation study; see README validation-status note.

## [1.0.1] — 2026-06-29

### Additions
- **Antecedent / Trigger field** (Section XIV) — structured capture of the A in
  A-B-C contingency, recommended by external review (Claude Opus 4).
- **Two-tier design note** in Purpose section — documents that graded scales
  (Section IX) and binary markers (Section X) are complementary levels of
  measurement, not redundant.
- **JSON export** — Download JSON button generates structured evaluation data
  for inter-rater reliability analysis and longitudinal tracking.
- **Live web version** at wiresplice.com/wafba/ — interactive form hosted on
  the Wiresplice public site, unlinked, for direct use and review.
- **Copyright and trademark** — © 2026 Wiresplice Studio, WAFBA™.
