# MCP & Skills Finder

Find the right MCP server, agent skill or plugin for any task, from inside Claude Code.

Ask things like:

- "Find me an MCP server for a Postgres database"
- "Is there a skill that writes unit tests?"
- "What plugins do code review?"

Claude searches a live directory of 13,900+ listings and recommends the best matches, with a link and the install command for each.

## Install

In Claude Code:

```
/plugin install mcp-skills-finder --marketplace aidevelopers2/mcp-skills-finder
```

Or from your shell:

```
claude plugin marketplace add aidevelopers2/mcp-skills-finder
claude plugin install mcp-skills-finder@mcp-skills-finder
```

## What's inside

- **MCP server** (remote, no sign-in): `https://www.claudemarket.ai/mcp-server/mcp` with three read-only tools: `search_mcp_servers`, `search_skills`, `search_plugins`.
- **Skill** `find-tools`: tells Claude when to search the directory and how to present results.

Read-only: it searches public directory listings. It doesn't install anything, access your accounts or call third-party services.

## Links

- Directory: https://www.claudemarket.ai
- Privacy: https://www.claudemarket.ai/privacy
- Terms: https://www.claudemarket.ai/terms
- Support: https://www.claudemarket.ai/contact

MIT licensed.
