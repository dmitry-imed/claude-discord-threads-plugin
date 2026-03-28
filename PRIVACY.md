# Privacy Policy

**discord-threads** is an open-source Claude Code plugin that runs entirely on your local machine.

## Data handling

- **No data collection.** The plugin does not collect, store, or transmit any personal data, telemetry, or analytics.
- **No external servers.** All processing happens locally. The only network connections are to the Discord API (to send and receive messages) and are initiated by your machine.
- **Credentials stay local.** Your Discord bot token is stored in `~/.claude/channels/discord/.env` on your machine with restricted file permissions (`chmod 600`). It is never logged, transmitted, or shared.
- **Messages are not stored.** Inbound and outbound messages pass through the MCP server in memory and are not written to disk, except for attachments you explicitly download (saved to `~/.claude/channels/discord/inbox/`).
- **Access control is local.** The access allowlist (`~/.claude/channels/discord/access.json`) is a local file managed by you.

## Discord API

The plugin connects to the [Discord Gateway and REST API](https://discord.com/developers/docs) using your bot token. Discord's own privacy policy applies to data processed by their platform: https://discord.com/privacy

## Third-party dependencies

None. The plugin uses only Node.js built-in modules.

## Contact

For questions, open an issue at https://github.com/axiumfoundry/claude-discord-threads-plugin/issues
