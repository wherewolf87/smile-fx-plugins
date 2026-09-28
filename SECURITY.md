# Security

## Report a problem

Please report security problems privately. Use **Report a vulnerability** on the Security tab of [this repository](https://github.com/wherewolf87/smile-fx-plugins/security), or reach SMILE-FX through https://smile-fx-ai.vercel.app. Do not open a public issue for a security problem.

Include the plugin and file, what you expected, what happened, and the steps to reproduce.

## What is in scope

- Files in this repository: skills, commands, plugin manifests, the marketplace file and the connector (`.mcp.json`) settings.
- A connector address in this repository that points somewhere unexpected.

Out of scope. Please report these to the company that runs them:

- A connected service's own MCP server (for example HubSpot or Slack): report to that company.
- Claude, Claude Code or Cowork: report to Anthropic.
- The `@modelcontextprotocol/server-pdf` package used by SMILE-FX PDF Viewer: report to its maintainers.

## How these plugins run

- Skills are written instructions. They run with the permissions of the app you use and the connectors you approve.
- Connectors are third-party servers. Each one signs in with your own account. Your app's permission settings decide whether each tool runs straight away or asks you first.
- SMILE-FX PDF Viewer starts a local server with `npx`, which downloads a package from npm the first time it runs.
- Review a plugin before you install it. Claude Code and Cowork show its skills and connectors first.

## Supported versions

Only the newest release receives fixes. Update with `/plugin marketplace update smile-fx-plugins` in Claude Code, or **Check for updates** in Cowork.
