# agentwikis-mcp (deprecated)

**This npm package is deprecated. Use the hosted Agent Wikis server instead: nothing to install.**

```
https://agentwikis.com/mcp
```

Streamable HTTP, read-only, free without a key. Setup commands for Claude Code, Codex, Grok Build, Hermes Agent, Cursor, ChatGPT and any other MCP client are on [agentwikis.com/for-agents](https://agentwikis.com/for-agents#mcp). For example, in Claude Code:

```bash
claude mcp add --transport http --scope user agentwikis "https://agentwikis.com/mcp"
```

The hosted server has everything this package had (`list_wikis`, `open_wiki`, `search`, `read_document`) plus the skills library, agent tools and routines. An optional [Agent Wikis Pro](https://agentwikis.com/pro) key goes into the app's connection as an `Authorization` header; the steps for each app are at [agentwikis.com/pro#connect](https://agentwikis.com/pro#connect).

The easiest way to add it, together with the AI Garage content server and its skills, is the free [AI Garage plugin](https://github.com/tonbistudio/aigarage-plugin).

## Existing installs

Version 0.2.3 still works: it is a local bridge that calls `agentwikis.com/api/*`. It gets no new features, and npm shows a deprecation notice on install. To switch, remove the `npx -y agentwikis-mcp` entry from your app's MCP config and add the hosted URL above under the same name, `agentwikis`.

## License

MIT
