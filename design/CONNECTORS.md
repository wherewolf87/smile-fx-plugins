# Connectors

## How tool references work

Skills name a kind of tool instead of one product. In plugin files these appear as placeholders such as `~~chat` or `~~CRM`. Any connector in that category works. The plugin's `.mcp.json` sets up the connectors listed under setup notes, and you can connect a different tool in the same category instead.

## Connectors for this plugin

| Category | Placeholder | Set up in this plugin | Other options |
|----------|-------------|-----------------|---------------|
| Chat | `~~chat` | Slack | Microsoft Teams |
| Design tool | `~~design tool` | Figma | Sketch, Adobe XD, Framer |
| Knowledge base | `~~knowledge base` | Notion | Confluence, Guru, Coda |
| Project tracker | `~~project tracker` | Linear, Asana, Atlassian (Jira/Confluence) | Shortcut, ClickUp |
| User feedback | `~~user feedback` | Intercom | Productboard, Canny, UserVoice, Dovetail |
| Product analytics | `~~product analytics` | None | Amplitude, Mixpanel, Heap, FullStory |

"Set up in this plugin" lists the connectors in this plugin's `.mcp.json`. "(blank address)" marks a placeholder you connect yourself.

## Setup notes

Every connector below signs in with your own account for that service. Nothing connects until you sign in, and installing the plugin does not sign you in to anything. In Cowork, open the plugin's **Connectors** tab. In Claude Code, run `/mcp`.

| Connector | Address | What you need | Check on September 27, 2026 | Notes |
|---|---|---|---|---|
| Slack | `https://mcp.slack.com/mcp` | Your own Slack workspace, with admin approval | Sign-in required (401) | Uses the sign-in app Slack publishes for Claude Code. A workspace admin must approve the Slack MCP app. |
| Figma | `https://mcp.figma.com/mcp` | Your own Figma account | Sign-in required (401) | None. |
| Linear | `https://mcp.linear.app/mcp` | Your own Linear account | Sign-in required (401) | None. |
| Asana | `https://mcp.asana.com/v2/mcp` | Your own Asana account | Sign-in required (401) | None. |
| Atlassian (Jira, Confluence) | `https://mcp.atlassian.com/v1/mcp` | Your own Atlassian account | Sign-in required (401) | None. |
| Notion | `https://mcp.notion.com/mcp` | Your own Notion account | Sign-in required (401) | None. |
| Intercom | `https://mcp.intercom.com/mcp` | Your own Intercom account | Sign-in required (401) | None. |
| Google Calendar | (blank) | Your own Google Calendar account | Placeholder | Blank on purpose, so it shows as "not configured" instead of an error. Connect Google Calendar from your Claude connector settings, or add Google's MCP server yourself. The skills use any calendar tool you connect. |
| Gmail | (blank) | Your own Gmail account | Placeholder | Blank on purpose, so it shows as "not configured" instead of an error. Connect Gmail from your Claude connector settings, or add Google's MCP server yourself. The skills use any email tool you connect. |

The check column is an anonymous request sent on September 27, 2026 with no account: it shows whether the address answered and asked for sign-in, not whether your account works. The full list for all plugins is in [CONNECTORS.md](../CONNECTORS.md) at the repository root.

Do not put patient health information (PHI) into Claude, a plugin or a connected tool unless your Claude plan and every connected service are covered by a signed Business Associate Agreement (BAA). Use de-identified examples when you test.
