# Virtuoso Agent Skills

Agent skills for the [Virtuoso](https://virtuoso.dev) component family. Each skill teaches coding agents (Claude Code, Codex, Cursor, OpenCode, and other [Agent Skills](https://agentskills.io) consumers) how to use a package correctly — component selection, core rules with reasoning, common patterns, and pitfalls — with the full package docs bundled as references.

| Skill | Covers |
| --- | --- |
| [react-virtuoso](react-virtuoso/SKILL.md) | Virtualized lists, grids, and tables (`Virtuoso`, `GroupedVirtuoso`, `VirtuosoGrid`, `TableVirtuoso`) |
| [message-list](message-list/SKILL.md) | Chat and AI conversation UIs (`VirtuosoMessageList`) |
| [data-table](data-table/SKILL.md) | Virtualized data grid with sorting, filtering, and column features (`@virtuoso.dev/data-table`) |
| [reactive-engine](reactive-engine/SKILL.md) | The `@virtuoso.dev/reactive-engine-*` state management family |

## Installation

### Agent Skills CLI (Codex, Cursor, OpenCode, and more)

```bash
npx skills add virtuoso-dev/skills --skill '*'
```

Or pick individual skills:

```bash
npx skills add virtuoso-dev/skills --skill react-virtuoso
```

### Claude Code

Install as a plugin from the source monorepo marketplace:

```text
/plugin marketplace add petyosi/react-virtuoso
/plugin install virtuoso-skills@virtuoso
```

### Codex plugin

```bash
codex plugin marketplace add petyosi/react-virtuoso --ref main --sparse .agents/plugins --sparse plugins/virtuoso-skills
codex plugin add virtuoso-skills@virtuoso
```

## Contributing

This repository is a generated mirror — the canonical source lives in the [react-virtuoso monorepo](https://github.com/petyosi/react-virtuoso) under `packages/virtuoso-skills/`, and the skill references are built from each package's docs. Please open issues and pull requests there; direct changes to this repository will be overwritten by the next sync.

## License

MIT — the skills cover both open-source packages and the commercially licensed `@virtuoso.dev/message-list` (the skill itself is free; the package requires a [license](https://virtuoso.dev/pricing/)).
