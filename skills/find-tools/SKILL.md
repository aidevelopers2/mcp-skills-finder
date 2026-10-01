---
name: find-tools
description: Use when the user wants to find, compare or choose an MCP server, agent skill or plugin for a task (for example "is there an MCP server for Postgres?", "find a skill that writes tests", "what plugin does code review?"). Searches a directory of 13,900+ listings with the mcp-skills-finder tools.
---

# Find MCP servers, skills and plugins

When the user is looking for a tool to extend their agent, search the directory instead of answering from memory. Listings change quickly and the directory is current.

## Which tool to call

- **MCP servers** (connect the agent to a database, API, browser, SaaS app): `search_mcp_servers`
- **Agent skills** (reusable instructions and workflows): `search_skills`
- **Plugins** (installable bundles of skills, commands and servers): `search_plugins`

If the request could match more than one type, call the relevant tools in turn.

## How to query

- Pass the task in a few plain words, not the whole sentence: "postgres database", "headless browser scraping", "write unit tests".
- Use `limit` 5 to 10 for a normal answer, up to 25 when the user wants a broad list.
- If nothing comes back, retry once with a shorter or more general query (for example "scraping" instead of "scrape JavaScript-heavy single page apps").

## How to answer

- Recommend the 2 to 4 best matches, not the whole list. Say in one line why each fits.
- Include each pick's link so the user can read the full listing, and the install command when the result has one.
- These tools only search. Never claim to have installed anything; if the user wants to install, give them the command to run.
