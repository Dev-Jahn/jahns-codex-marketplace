# Jahn's Codex Marketplace

Personal Codex plugin registry maintained by [Jahn](https://github.com/Dev-Jahn).

## Install

```bash
codex plugin marketplace add Dev-Jahn/jahns-codex-marketplace
codex plugin add hippo@jahns-codex-marketplace
codex plugin add khala-network-codex@jahns-codex-marketplace
codex plugin add hwp-hwpx-editor@jahns-codex-marketplace
codex plugin add jahns-stl@jahns-codex-marketplace
```

Start a new Codex session after installation. Review and trust installed hooks with
`/hooks`; Codex does not run untrusted plugin hooks until their exact hash is approved.

## Update

```bash
codex plugin marketplace upgrade jahns-codex-marketplace
codex plugin add hippo@jahns-codex-marketplace
codex plugin add khala-network-codex@jahns-codex-marketplace
codex plugin add hwp-hwpx-editor@jahns-codex-marketplace
codex plugin add jahns-stl@jahns-codex-marketplace
```

The registry pins each plugin to an exact Git commit. Each source repository's workflow updates
its own entry after validation on `main` where configured; HWP/HWPX Editor releases are registered manually.

## Available plugins

| Plugin | Description | Source |
|---|---|---|
| `hippo` | Project memory, task registry, outcome ledger and background clerks | [Dev-Jahn/hippocampus](https://github.com/Dev-Jahn/hippocampus) |
| `khala-network-codex` | Durable mail and streams between Codex and Claude Code sessions, with native Codex doorbells | [Dev-Jahn/khala-network-codex](https://github.com/Dev-Jahn/khala-network-codex) |
| `hwp-hwpx-editor` | HWP/HWPX text, bullets, tables, pictures and formatting, with validation and PDF rendering | [Dev-Jahn/hwp-hwpx-editor](https://github.com/Dev-Jahn/hwp-hwpx-editor) |
| `jahns-stl` | Writing guide for agents: no invented jargon, and text that is clear to a reader who was not there, in any language | [Dev-Jahn/jahns-stl](https://github.com/Dev-Jahn/jahns-stl) |

Khala setup and automatic receive modes are documented in the plugin's README. In ordinary
standalone Codex, hooks provide active-turn reminders; `khala-codex run` also supports idle wake.

## License

MIT
