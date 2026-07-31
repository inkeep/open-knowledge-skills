# Open Knowledge Skills

Agent Skills published by [Open Knowledge](https://openknowledge.ai). Each skill teaches
an agent one repeatable task, and every one of them is plain markdown you can read before
you install it.

`skills/` is generated. The skills there are projected from the Open Knowledge source
tree, so each directory name matches its `SKILL.md` frontmatter `name`.

## Install

Add this repository as a Claude Code plugin marketplace, then install what you want:

```bash
/plugin marketplace add inkeep/open-knowledge-skills
/plugin install open-knowledge@open-knowledge-skills
```

`open-knowledge` is the platform skill: it teaches an agent to read, search, link, and
write markdown through Open Knowledge's MCP server. The rest are optional packs. Run
`/plugin marketplace list` to see everything this repository publishes.

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
