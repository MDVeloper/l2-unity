# Agent instructions

## Unity

- Use documentation: https://github.com/Unity-Technologies/skills
- Use official Unity skills: https://github.com/Unity-Technologies/skills
- Prefer Unity CLI over the deprecated in-Editor MCP server: https://docs.unity.com/en-us/unity-cli/replace-mcp-server-unity-cli

### Deprecation note (official)

Unity deprecated the MCP server in the in-editor AI assistant package (`com.unity.ai.assistant`). Use the **Unity CLI** instead:

- Prefer `unity command` / `unity eval` when the agent can run shell commands (faster, fewer tokens).
- Use `unity mcp` only when MCP mode is needed (agents that cannot reliably run shell commands).
- Install skills with `unity skill install <agent-name>` (or `npx skills add Unity-Technologies/skills`).

Docs: https://docs.unity.com/en-us/unity-cli

When working on Unity workflows in this repo, prefer official Unity skills + Unity CLI. Do not set up or rely on the deprecated in-Editor AI Assistant MCP server.
