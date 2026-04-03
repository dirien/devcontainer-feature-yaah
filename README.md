# devcontainer-feature-yaah

A Dev Container feature to install [yaah](https://github.com/dirien/yet-another-agent-harness) (Yet Another Agent Harness) — a Go agent harness for AI coding agents with hooks, MCP server, session tracking, and config generation.

## Usage

Add the following to your `devcontainer.json`:

```json
{
    "features": {
        "ghcr.io/dirien/devcontainer-feature-yaah/yaah:0": {}
    }
}
```

## Options

| Option  | Type   | Default    | Description                                                                                          |
|---------|--------|------------|------------------------------------------------------------------------------------------------------|
| `version` | string | `"latest"` | Version of yaah to install (e.g., `0.3.3`). Set to `latest` for the latest release.                 |
| `agent`   | string | `""`       | Agent profile to generate config for (e.g., `claude`, `copilot`, `opencode`, `codex`). Leave empty to skip. |

### Pin to a specific version with agent config

```json
{
    "features": {
        "ghcr.io/dirien/devcontainer-feature-yaah/yaah:0": {
            "version": "0.3.3",
            "agent": "claude"
        }
    }
}
```
