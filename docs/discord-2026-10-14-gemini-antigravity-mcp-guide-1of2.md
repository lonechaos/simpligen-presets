🤖 **Getting Started: Antigravity / Gemini CLI + SimpliGen**
SimpliGen ships an MCP server, which lets Google Antigravity and Gemini CLI drive your image and video generation directly. Describe the shot in chat, and the agent can find the preset, set the options, run the job, and retrieve the result.

1️⃣ **What you need**
- SimpliGen installed and running. The MCP server talks to the live app, so keep it open.
- Node.js installed. The server runs through `npx`.
- Google Antigravity (IDE or CLI) or Gemini CLI.
- At least one preset ready to run locally, or cloud credits.

The Gemini app on the web (gemini.google.com) can't connect: it only accepts remote servers, and SimpliGen's server runs on your own PC.

2️⃣ **Connect**
1. In SimpliGen, open **Settings → Connect an agent**.
2. Pick **Google Antigravity** or **Gemini CLI**, then select **Install**.
3. Restart Antigravity or Gemini CLI.

SimpliGen issues a pairing token and writes the configuration for you. In Gemini CLI, type `/mcp` to check that `simpligen` shows as CONNECTED.

3️⃣ **Manual setup**
Add this entry, replacing `sg-agent-...` with your pairing token from **Settings → Connect an agent**:
```json
{
  "mcpServers": {
    "simpligen": {
      "command": "npx",
      "args": ["-y", "@simpligen/mcp"],
      "env": { "SIMPLIGEN_TOKEN": "sg-agent-..." }
    }
  }
}
```
- **Antigravity:** `~/.gemini/config/mcp_config.json` (Windows: `C:\Users\<you>\.gemini\config\mcp_config.json`). The IDE and the CLI share this file.
- **Gemini CLI:** `~/.gemini/settings.json`. Gemini Code Assist in VS Code reads the same file.

Preserve any existing configuration: if the file already has an `mcpServers` section, add the `simpligen` entry inside it. Restart after saving.

Keep the token in the `env` block. Gemini CLI hides environment variables with TOKEN in their name from MCP servers, so setting `SIMPLIGEN_TOKEN` in your system environment instead won't work.

🔒 Treat the token like a password. It gives whoever has it control of your SimpliGen. Don't paste it in chat or commit it to a repository.
