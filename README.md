# Open Knowledge Skills

Agent Skills published by [Open Knowledge](https://openknowledge.ai). Each skill teaches
an agent one repeatable task, and every one of them is plain markdown you can read before
you install it.

`skills/` is generated. The skills there are projected from the Open Knowledge source
tree, so each skill directory's leaf name matches its `SKILL.md` frontmatter `name`.
The layout groups by role:

- `skills/core/` holds the platform and meta skills.
- `skills/starter-packs/<pack>/` holds one folder per starter pack: the pack's
  orientation skill, its member skills as sibling directories, and a README
  explaining how they interact.

## Install

Add this repository as a Claude Code plugin marketplace, then install what you want:

```bash
/plugin marketplace add inkeep/open-knowledge-skills
/plugin install open-knowledge@open-knowledge-skills
```

`open-knowledge` is the platform skill: it teaches an agent to read, search, link, and
write markdown through Open Knowledge's MCP server. The rest are optional packs.

## What's published here

Install a pack by name, the same way: `/plugin install <pack>@open-knowledge-skills`.

### Core

| Skill | What it does |
| --- | --- |
| `open-knowledge` | The runtime contract for working inside an Open Knowledge project: reading, searching, linking, and writing markdown through its MCP server. |
| `open-knowledge-discovery` | What Open Knowledge is, how to install it on a repository, and how to share a project with collaborators. |
| `open-knowledge-write-skill` | Authoring a new Agent Skill: the frontmatter contract, progressive-disclosure structure, and how to install it into your editors. |

### Starter packs

Each pack ships an orientation skill that explains how to work in that project shape. Some
add task skills alongside it.

| Pack | Orientation skill | Also ships |
| --- | --- | --- |
| `software-lifecycle` | proposals to decisions to specs to postmortems | `frame-a-proposal`, `write-a-spec`, `record-a-decision`, `write-a-postmortem`, `review-a-design` |
| `knowledge-base` | source-grounded research: sources to research to articles | `research-with-sources`, `consolidate-notes` |
| `codebase-wiki` | an agent-authored, source-grounded wiki of the surrounding codebase | |
| `personal-crm` | a typed-entity vault of people, companies, and meetings, each with a rewritable summary and an append-only timeline | |
| `note-taking` | a flat notes folder plus a daily journal, for when you just want to write | |
| `writing-workflow` | a three-stage drafting flow: ideas to drafts to published | |
| `worldbuilding` | a fiction encyclopedia of characters, settings, factions, and lore | |
| `okf-knowledge-base` | a knowledge base conformant with Google's Open Knowledge Format from the first commit | |

The task skills stand on their own. `write-a-spec` and `record-a-decision` do not need an
Open Knowledge project, or the rest of their pack, to be useful.

You can also copy any skill straight into your agent's skills folder
(`.claude/skills/`, `.cursor/skills/`, `.codex/skills/`, or the vendor-neutral
`.agents/skills/`). Open Knowledge can install and update them for you, and keeps their
version history.

## Writing your own

`template/SKILL.md.example` is a starting point. The field that matters most is
`description`: it is a routing rule, not a title, and it is what both skills.sh and the
host agent match on to decide whether to load the skill at all.

Read [CONTRIBUTING.md](./CONTRIBUTING.md) before opening a PR.

## License

[MIT](./LICENSE)
