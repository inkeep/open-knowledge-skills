# Codebase Wiki

An OpenKnowledge starter pack that turns a repo into an agent-maintained wiki:
source-grounded articles about the surrounding codebase, regenerated as the
code changes rather than rotting beside it.

## Skills

| Skill | What it does |
|---|---|
| `codebase-wiki` | How to author and refresh wiki articles: grounding every claim in the source tree, structuring pages around subsystems, and refreshing stale articles instead of appending to them. |

## Install

- Seed a project: `ok seed --pack codebase-wiki`
- Claude Code plugin: `/plugin install codebase-wiki@open-knowledge-skills`
