# Knowledge Base

An OpenKnowledge starter pack for source-grounded knowledge work. The flow is
external sources in, research on top, consolidated articles out: capture
sources verbatim, research against them, then promote settled findings to
canonical articles.

## Skills

The orientation skill routes; the two member skills carry the procedures.

| Skill | Role |
|---|---|
| `knowledge-base` | Orientation: what lives where in the project and which member skill handles the request. |
| `research-with-sources` | Investigate a topic against preserved sources and write a draft-status research article, citing every claim. |
| `consolidate-notes` | After a decision lands, promote research into a stable-status canonical article with a `supersedes:` chain. |

`research-with-sources` produces `status: draft` articles;
`consolidate-notes` is the only path that turns them into `status: stable` canonical knowledge. The orientation
skill exists so an agent picks the right one instead of improvising.

## Install

- Seed a project (folders, templates, and all three skills): `ok seed --pack knowledge-base`
- Claude Code plugin (all three skills): `/plugin install knowledge-base@open-knowledge-skills`
