# claude_plugins

A personal marketplace of Claude Code plugins.

## Installation

### 1. Add the marketplace

```shell
# Claude Code slash command
/plugin marketplace add mcbottcher/claude_plugins

# Or directly via CLI
claude plugin marketplace add mcbottcher/claude_plugins
```

### 2. Install a plugin

```shell
# Claude Code slash command
/plugin install <plugin-name>@mcbottcher-plugins

# Or directly via CLI
claude plugin install <plugin-name>@mcbottcher-plugins
```

By default, plugins are installed at user scope (available across all projects). Use `--scope` to change this:

| Scope | Flag | Effect |
|---|---|---|
| User (default) | `--scope user` | Available in all projects |
| Project | `--scope project` | Shared with team via `.claude/settings.json` |
| Local | `--scope local` | Project-only, gitignored |

```shell
# Claude Code slash command
/plugin install <plugin-name>@mcbottcher-plugins --scope project

# Or directly via CLI
claude plugin install <plugin-name>@mcbottcher-plugins --scope project
```

## Available plugins

### `commit`

Stage all changes and commit using conventional commits style.

```shell
# Claude Code slash command
/plugin install commit@mcbottcher-plugins --scope project

# Or directly via CLI
claude plugin install commit@mcbottcher-plugins --scope project
```
