# Jahn's Codex Marketplace

Personal Codex plugin registry maintained by [Jahn](https://github.com/Dev-Jahn).

## Install Waystone

```bash
codex plugin marketplace add Dev-Jahn/jahns-codex-marketplace
codex plugin add waystone@jahns-codex-marketplace
```

Start a new Codex session after installation. Review and trust Waystone's installed hooks with
`/hooks`; Codex does not run untrusted plugin hooks until their exact hash is approved.

## Update

```bash
codex plugin marketplace upgrade jahns-codex-marketplace
codex plugin add waystone@jahns-codex-marketplace
```

The registry pins each plugin to an exact Git commit. Waystone's release workflow updates that pin
after a release reaches its `main` branch.

## Available plugins

| Plugin | Description | Source |
|---|---|---|
| `waystone` | SSOT-anchored agentic development workflow for Claude Code and Codex | [Dev-Jahn/waystone](https://github.com/Dev-Jahn/waystone) |

## License

MIT
