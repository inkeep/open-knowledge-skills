# Contributing to Open Knowledge Skills

This repository is maintained by Inkeep and mirrored here with Copybara.

## `skills/` is generated

The `skills/` directory is projected from Open Knowledge's source tree — it is
not editable here. A PR that changes a file under `skills/` cannot be accepted,
because the next mirror sync overwrites it from source. To change a shipped
skill, open an issue describing the change and a maintainer will make it at the
source.

Everything else in this repository (`template/`, `README.md`, this file, the
workflows) is editable here in the normal way.

## How Public PRs Flow

1. Open a PR against this repository (outside `skills/` — see above).
2. Automation mirrors the PR into Inkeep's maintainer review flow.
3. Once accepted, the change syncs back here and your PR is closed automatically
   (not merged—the change lands through the mirror sync).

## What to Expect

- The bridge waits for an Inkeep maintainer to approve its protected environment
  before it imports your change.
- Maintainer comments are not automatically mirrored back to the public PR. If
  you do not hear back within a few business days, commenting on your PR is the
  right way to follow up.
- Accepted changes land here with the original contributor's authorship
  preserved.
