![Blue Triangle](assets/logo-full.png)

# Blue Triangle MCP

Blue Triangle web performance & revenue analytics via MCP — query Core Web
Vitals, errors, resource timing, and conversion/revenue data across your
site accounts directly from an AI assistant.

- **Endpoint:** `https://mcp.bluetriangle.com/mcp`
- **Auth:** OAuth — your client will prompt you to log in on first connection. No API keys to manage.

## What you can do with it

- Query Core Web Vitals (CWV) and RUM metrics across site accounts
- Surface errors and resource-timing data
- Report on conversion/revenue impact of performance issues

## Installation

### Claude
Add as a custom connector:
1. In Claude, go to **Settings → Connectors → Add custom connector**.
2. Enter the URL: `https://mcp.bluetriangle.com/mcp`.
3. Complete the OAuth login when prompted.

### Cursor
Add to your MCP config (e.g. `~/.cursor/mcp.json` or your project's `.cursor/mcp.json`):

```json
{
  "mcpServers": {
    "blue-triangle-mcp": {
      "url": "https://mcp.bluetriangle.com/mcp"
    }
  }
}
```

Cursor will prompt for OAuth login on first use. (See `mcp.json` and
`.cursor-plugin/plugin.json` in this repo for the same config, ready to copy.)

### ChatGPT / Codex
Add the endpoint `https://mcp.bluetriangle.com/mcp` as a connector in your
ChatGPT/Codex settings; OAuth is handled automatically.

### GitHub Copilot
Listed in the [Official MCP Registry](https://github.com/modelcontextprotocol/registry)
(see `registry/server.json`) — searchable and installable directly from
Copilot's MCP registry integration, no extra setup in this repo required.

## About this repository

This repository contains the plugin/registry manifests and installation
instructions for the Blue Triangle MCP server. It does **not** contain the
server's source code — the server runs as a private, closed-source service
at `https://mcp.bluetriangle.com/mcp`.

## Support

- MCP endpoint: https://mcp.bluetriangle.com/mcp
- Issues with this listing: open an issue in this repo
- Issues with the server itself: support@bluetriangle.com

