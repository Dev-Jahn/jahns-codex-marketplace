# Jahn's Codex Marketplace

Personal Codex plugin registry maintained by [Jahn](https://github.com/Dev-Jahn).

## Install

```bash
codex plugin marketplace add Dev-Jahn/jahns-codex-marketplace
codex plugin add hippo@jahns-codex-marketplace
codex plugin add khala-network-codex@jahns-codex-marketplace
```

Start a new Codex session after installation. Review and trust installed hooks with
`/hooks`; Codex does not run untrusted plugin hooks until their exact hash is approved.

## Update

```bash
codex plugin marketplace upgrade jahns-codex-marketplace
codex plugin add hippo@jahns-codex-marketplace
codex plugin add khala-network-codex@jahns-codex-marketplace
```

The registry pins each plugin to an exact Git commit. Each source repository's workflow updates
its own entry after validation on `main`.

## Available plugins

| Plugin | Description | Source |
|---|---|---|
| `hippo` | Project memory, task registry, outcome ledger and background clerks | [Dev-Jahn/hippocampus](https://github.com/Dev-Jahn/hippocampus) |
| `khala-network-codex` | Durable mail and streams between Codex and Claude Code sessions, with native Codex doorbells | [Dev-Jahn/khala-network-codex](https://github.com/Dev-Jahn/khala-network-codex) |

Khala setup and automatic receive modes are documented in the plugin's README. In ordinary
standalone Codex, hooks provide active-turn reminders; `khala-codex run` also supports idle wake.

## License

MIT
