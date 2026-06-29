# WAFBA

**Wiresplice AI Functional Behavioral Assessment**
Version 1.0 · Released 2026-06-29

A structured instrument for evaluating the *functional behavior* of AI systems
during real-world work.

Developed by Kristi Gilleland, RN, MCSE, CIW-Master · Wiresplice Studio

---

## What this is

WAFBA assesses how an AI system actually behaves when given a real task in a
real execution environment — not how a model scores on a benchmark in isolation.

It is built on the clinical **Functional Behavioral Assessment (FBA)** model: a
method for understanding the behavior of complex systems you cannot directly
inspect, by observing behavior in context across repeated trials. The FBA was
developed for humans — historically the first opaque complex systems we needed
to manage without dissection. The same epistemics apply to AI systems whose
internals are not legible to the operator.

WAFBA evaluates the **complete working system** — model, execution
configuration, harness, and task context — because the same model weights behave
differently under different scaffolding. The harness is part of the patient.

**WAFBA is not an intelligence test or a benchmark.**

## Who it's for

- **AI operators and engineers** evaluating models and agents before and during
  deployment — establishing baselines, documenting failure modes, deciding what
  a system can be trusted to do unsupervised.
- **Clinical and institutional staff** (nurses, physicians, informatics leads)
  who may need to assess and document an AI system entering a real workflow,
  using an instrument whose form their training already parses.

## What's in this repository

| Path | Contents |
|------|----------|
| `docs/WAFBA-spec.md` | The instrument specification — every section, field, rating domain, and behavioral marker, as a readable document. |
| `wafba.html` | The working assessment form. Single-file HTML/JS. Open in a browser, complete an evaluation, generate a report. No server, no dependencies, no data leaves the page. |
| `CHANGELOG.md` | Version history. |
| `CITATION.cff` | Citation metadata. |
| `LICENSE` | CC BY-SA 4.0. |

A live version of the form is also hosted at **[wiresplice.com/wafba/](https://www.wiresplice.com/wafba/)**.

## Using the form

The form is available in two ways:

- **Live web version** — open [wiresplice.com/wafba/](https://www.wiresplice.com/wafba/) in any browser. Fill, generate a report, print to PDF. Nothing is transmitted or stored.
- **Offline version** — open `wafba.html` from this repository in any modern browser. Same form, same behavior, no server needed.

The form runs entirely client-side — nothing is transmitted, stored remotely, or logged. Complete the sections, generate a report, and copy or print it. To capture a structured record, use **Download JSON** to export the evaluation as structured data, or save the generated report alongside your own evaluation log.

## The instrument at a glance

WAFBA captures, for each evaluation:

- **System identity** — advertised model *and* execution configuration
  (reasoning level, context window, temperature, memory, autonomy), kept
  separate because the nameplate is not the system.
- **Provenance confidence** — how certain the evaluator is that the advertised
  model is the one actually evaluated. A first-class field, because operators do
  not always have full visibility into the execution stack.
- **Functional behavioral ratings** (1–5) across eight domains: goal
  maintenance, authority calibration, scope control, cognitive flexibility,
  reality orientation, environmental preservation, recovery, and supervision
  burden.
- **Behavioral markers** — a checklist of observable failure modes (authority
  inversion, configuration fixation, self-destructive execution, hallucinatory
  construction, perseveration, and others), drawn from documented real-world
  agent incidents.
- **Operator observations, evaluation conditions, overall functional
  impression, and consistency-with-baseline** — the subjective and longitudinal
  layers a benchmark cannot capture.

## Important: validation status

WAFBA is an **operational field instrument**, not a clinically validated
psychometric scale. As of v1.0 it has **not** undergone formal inter-rater
reliability or validity studies. It is offered as a structured, repeatable
assessment framework based on operational experience. Treat its outputs as
documented operator judgment, not as a validated clinical measure. Independent
validation work is welcomed and, under this license, must be shared back openly
(see License).

This is not legal, medical, or compliance advice. Institutions adopting WAFBA in
a governed setting are responsible for their own review.

## License

Licensed under **CC BY-SA 4.0**. You may use, adapt, and build on WAFBA —
including commercially — provided you credit Kristi Gilleland / Wiresplice Studio
and license your derivatives under the same terms. Improvements to the
instrument return to the commons. See [`LICENSE`](LICENSE).

## Citation

If you use WAFBA in research or practice, please cite it. See
[`CITATION.cff`](CITATION.cff). A versioned DOI is minted per release via Zenodo
(add the badge once the first release is archived).

---

*Wiresplice Studio — local-first AI. Rome, Georgia.*
