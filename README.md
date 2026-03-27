# claude-discord-threads-plugin

A Claude Code plugin marketplace with a Discord plugin that adds per-session thread routing for multi-session setups.

## Plugins

- **discord-threads** — Discord messaging bridge with session-isolated threads. When multiple Claude Code sessions run simultaneously, each session gets its own Discord thread so messages route to the correct session.

## Installation

```
/plugin marketplace add dmitry-imed/claude-discord-threads-plugin
/plugin install discord-threads@dmitry-plugins
```

Then launch Claude Code with the channel:

```sh
claude --channels plugin:discord-threads@dmitry-plugins
```

See [plugins/discord-threads/README.md](plugins/discord-threads/README.md) for full setup instructions.
