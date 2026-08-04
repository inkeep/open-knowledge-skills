# Software Lifecycle

An OpenKnowledge starter pack for engineering-process writing: proposals,
specs, decisions, postmortems, and design reviews, each with its own scenario
skill so the discipline travels with the document type.

## Skills

The orientation skill routes; the five member skills carry the procedures.

| Skill | Role |
|---|---|
| `software-lifecycle` | Orientation: what lives where in the project and which scenario skill handles the request. |
| `frame-a-proposal` | A change needs designing and arguing before anyone builds it. |
| `write-a-spec` | An accepted proposal needs scoping into an implementable spec. |
| `record-a-decision` | A decision was actually made and needs its context and consequences preserved. |
| `write-a-postmortem` | An incident happened and the team needs a blameless write-up. |
| `review-a-design` | An existing proposal, spec, or decision needs pressure-testing for soundness. |

The scenario skills chain: a proposal becomes a spec, specs and proposals
produce decisions, and any of them can be pressure-tested with
`review-a-design`. The orientation skill exists so an agent picks the right
scenario instead of improvising a document type.

## Install

- Seed a project (folders, templates, and all six skills): `ok seed --pack software-lifecycle`
- Claude Code plugin (all six skills): `/plugin install software-lifecycle@open-knowledge-skills`
