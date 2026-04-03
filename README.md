# Spacelift Flows - Agent Skills

A Claude Code plugin marketplace that provides auto-loaded guidance for building Spacelift Flows apps.

When installed, Claude automatically loads the Flows app development skill whenever it detects you're working on a Flows app project (TypeScript project using `@slflows/sdk`). No slash command needed - it just works.

## Installation

### Claude Code

```bash
# Add the marketplace (one-time)
claude plugin marketplace add spacelift-io/flows-apps-agent-skills

# Install the plugin
claude plugin install flows-app-dev@spacelift-flows
```

After installation, Claude will automatically use the Flows app development guidance whenever you're working on a Flows app.

## Updating

Claude Code auto-updates plugins at startup. To manually update:

```
/plugin marketplace update spacelift-flows
/plugin update
```

## Developing

To test the plugin locally:

```bash
claude --plugin-dir ./plugins/flows-app-dev
```

To validate the plugin structure:

```bash
claude plugin validate ./plugins/flows-app-dev
```

## Versioning

This plugin follows semantic versioning. The version is tracked in `plugins/flows-app-dev/.claude-plugin/plugin.json`.

When updating the skill content, always bump the version - Claude Code uses the version to detect updates and won't pick up content changes without a version bump.
